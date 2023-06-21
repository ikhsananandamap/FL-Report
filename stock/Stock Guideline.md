1. Adjust the template between sales raw data and SKU. **Note: One file for one country**
2. **Make a copy** the script to your Google Drive [Stock Report ID](https://colab.research.google.com/drive/1FV-2CGmtSYcRHD3vKf9NyKClNxhlSz0K?usp=sharing) [Stock Report PH](https://colab.research.google.com/drive/1L2XXCHXNt1FYJ98itjp0eEsdWpvl-GnA?usp=sharing)
3. Upload your file to Google Colaboratory
4. Adust the name of your Stock and SKU Files
```python
#Import Data
file_name = 'Stock 19 06 2023.xlsx'
data_raw = pd.read_excel(file_name, sheet_name='Sheet1')
data_sku_product = pd.read_excel('SKU PHP.xlsx', sheet_name='Product')
data_sku_sales = pd.read_excel('SKU PHP.xlsx', sheet_name='Sales')
data_sku_inventory = pd.read_excel('SKU PHP.xlsx', sheet_name='Inventory')
data_sku_mapping = pd.read_excel('SKU PHP.xlsx', sheet_name='Mapping')
data_sku_exclude = pd.read_excel('SKU PHP.xlsx', sheet_name='Exclude')
data_stock = pd.read_excel('FL PHP Database - 2023 (Weekly).xlsx', sheet_name='Act_EOP')

#Export Data
data_final.to_excel("Hasil Stock 150423.xlsx", sheet_name = 'FINAL')
```
5. Run the script through Runtime > Run All
6. Download the results file
