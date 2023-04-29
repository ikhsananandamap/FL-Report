
1. Adjust the data template. **Note: One file for one country and from Wk 01 to Wk 12**
2. **Make a copy** the script to your Google Drive [Brand Report](https://colab.research.google.com/drive/1_6Fa5kVcGmXgBx9bgPz0YK_D-cwZyhfa?usp=sharing)
3. Upload your file to Google Colaboratory
4. Adust the name of your Input Data and Output Files
```python
#Read Data
data_raw = pd.read_excel('Week 1 12.xlsx', sheet_name='Sheet1')

#export
file_name = data_brand['Brand'][i] + ' FL ID- Weekly Report 2023 220423' + '.xlsx'
```
5. ***Rename your column*** where for Sales Quantity from **Wk to Qty**, End Stock from **Wk to Stk**, and Sell Rate from **Wk to St**
6. Run the script through Runtime > Run All
7. Download the results file
8. The output file of the program has deleted rows of data with a article of 0 and movement type 641,642, 351 
