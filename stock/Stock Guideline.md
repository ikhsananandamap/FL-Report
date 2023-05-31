1. Adjust the template between sales raw data and SKU. **Note: One file for one country**
2. **Make a copy** the script to your Google Drive [Stock Report ID](https://colab.research.google.com/drive/1FV-2CGmtSYcRHD3vKf9NyKClNxhlSz0K?usp=sharing) [Stock Report PH](https://colab.research.google.com/drive/1NiRHM1rcqM_QdPJhpwt_dOepj7ENXmOq?usp=sharing)
3. Upload your file to Google Colaboratory
4. Adust the name of your Stock and SKU Files
```python
#Import Data
data_raw = pd.read_excel('Stock 150423.xlsx', sheet_name='RAW')
data_sku_product = pd.read_excel('SKU.xlsx', sheet_name='Product')
data_sku_sales = pd.read_excel('SKU.xlsx', sheet_name='Sales')
data_sku_inventory = pd.read_excel('SKU.xlsx', sheet_name='Inventory')
data_sku_mapping = pd.read_excel('SKU.xlsx', sheet_name='Mapping')

#Export Data
data_final.to_excel("Hasil Stock 150423.xlsx", sheet_name = 'FINAL')
```
5. Run the script through Runtime > Run All
6. Download the results file
