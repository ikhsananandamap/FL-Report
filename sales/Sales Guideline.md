1. Adjust the template between sales raw data and SKU
2. **Make a copy** the script to your Google Drive [Sales Report](https://colab.research.google.com/drive/1AtVvT0af-VlrxdxtPxPp1KJrIuZ44xj8?usp=sharing)
3. Upload your file to Google Colaboratory
4. Adust the name of your Sales and SKU Files
```python
#Import Data
data_raw = pd.read_excel('Sales 150423.xlsx', sheet_name='RAW')
data_sku_product = pd.read_excel('SKU.xlsx', sheet_name='Product')
data_sku_sales = pd.read_excel('SKU.xlsx', sheet_name='Sales')
data_sku_inventory = pd.read_excel('SKU.xlsx', sheet_name='Inventory')

#Export Data
data_final.to_excel("Hasil Sales 150423.xlsx", sheet_name = 'FINAL')
```
5. Adjust the Gen.Art based on the selected country
If you want to make a report from Indonesian data you need to untag the FL Indonesia like this : 
```python
#Division to Color
#FL Indonesia
genarticle_loc = data_sku_product.index[data_sku_product['Gen.art']==data_raw['Genarticle'][i]].tolist()
  
#FL Philippines
# genarticle_loc = data_sku_product.index[data_sku_product['Gen.art (PH)']==data_raw['Genarticle'][i]].tolist()
```
If you want to make a report from Philippines data you need to untag the FL Philippines like this : 
```python
#Division to Color
#FL Indonesia
#genarticle_loc = data_sku_product.index[data_sku_product['Gen.art']==data_raw['Genarticle'][i]].tolist()
  
#FL Philippines
genarticle_loc = data_sku_product.index[data_sku_product['Gen.art (PH)']==data_raw['Genarticle'][i]].tolist()
```
6. Run the script through Runtime > Run All
7. Download the results file
