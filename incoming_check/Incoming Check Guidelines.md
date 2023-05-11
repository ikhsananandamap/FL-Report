1. Adjust the template of buying plan. **Note: One file for one season except 2022**
2. Note that the original and updated buying plan 2022 contains Jun'22 not Jun-22 and adjust the updated column with final intro column
3. **Make a copy** the script to your Google Drive [Incoming Check](https://colab.research.google.com/drive/1uBd4D0JV7SJ6nk4_YUU1REzP3RCDyuBe?usp=sharing)
4. Upload your file to Google Colaboratory
5. Adust the name of your Buying Plan
```python
#Read All Data
buying_plan_fw_fw_2023 = pd.read_excel('Buying Plan FW23 Footwear Python.xlsx', sheet_name='Sheet1')
buying_plan_fw_app_2023 = pd.read_excel('Buying Plan FW23 App Accs Python.xlsx', sheet_name='Sheet1')
buying_plan_ss_fw_2023 = pd.read_excel('Buying Plan SS23 Footwear Python.xlsx', sheet_name='Sheet1')
buying_plan_ss_app_2023 = pd.read_excel('Buying Plan SS23 App Accs Python.xlsx', sheet_name='Sheet1')
buying_plan_ss_2022 = pd.read_excel('Buying Plan SS22 Python.xlsx', sheet_name='Sheet1')
buying_plan_fw_2022 = pd.read_excel('Buying Plan FW22 Python.xlsx', sheet_name='Sheet1')
```
5. Steps to run the script : 
- Run the "Run This" Section
- After that, if the current season is Spring Summer, just run the "Season SS" and "HAD Files" Section
- if the current season is Fall Winter, just run the "Season FW" and "HAD Files" Section
6. Download the results file
7. The output file of the program has deleted rows of Canceled, TBA, #N/A inside Updated column and Blanks from MAP Brand column
