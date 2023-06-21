1. Adjust the template between sales raw data and SKU. **Note: One file for one country**
2. **Make a copy** the script to your Google Drive [Sales Report ID](https://colab.research.google.com/drive/1AtVvT0af-VlrxdxtPxPp1KJrIuZ44xj8?usp=sharing) [Sales Report PH](https://colab.research.google.com/drive/1sQsXicTRCgYduOvb0YFz4eLf4v7msp5A?usp=sharing)
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
5. Run the script through Runtime > Run All
6. Download the results file
7. The output file of the program has deleted rows of data with a total sales quantity of 0 
