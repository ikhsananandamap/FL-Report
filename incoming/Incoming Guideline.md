1. Adjust the template between sales raw data and SKU. **Note: One file for one country**
2. **Make a copy** the script to your Google Drive [Incoming Report ID](https://colab.research.google.com/drive/1LHcd-Ai4Bp_1DihRL2S0umqxJGROWuLP?usp=sharing) [Incoming Report PH](https://colab.research.google.com/drive/1Fz4YXPlozHd8U5DFVGSweM6EYc1Dmh51?usp=sharing)
3. Upload your file to Google Colaboratory
4. Adust the name of your Incoming, Buying Plan, and SKU Files
```python
#Import Data
data_raw = pd.read_excel('Incoming 10423.xlsx', sheet_name='Sheet1')
data_sku_product = pd.read_excel('SKU.xlsx', sheet_name='Product')
data_sku_sales = pd.read_excel('SKU.xlsx', sheet_name='Sales')
data_sku_inventory = pd.read_excel('SKU.xlsx', sheet_name='Inventory')
data_sku_mapping = pd.read_excel('SKU.xlsx', sheet_name='Mapping')
data_buying_plan = pd.read_excel('Buying Plan.xlsx', sheet_name='Sheet1')


#Export Data
data_final.to_excel("Hasil Incoming 10423.xlsx", sheet_name = 'FINAL')
```
5. Run the script through Runtime > Run All
6. Download the results file
