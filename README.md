# Identifying-side-Effects-and-Evaluating-the-effectiveness-of-Drugs







# Download All Data sets and files from this link - https://drive.google.com/drive/folders/1OjjUttHrQ5v1bJqwVkyGWGEoCnKVFP0n?usp=sharing

Business objective:- The aim of this project is to create a text-mining model to evaluate the effectiveness and detect potential side effects from online customer reviews on specific prescriptive drugs

## Before accessing the files please go through the description. ##

File name: project 4  Drug extraction
Description: 
The python code is used to extract data from webmd.com and the library that is used is the code is selenium and beautiful soup.
Output : Drug.csv 



File name: project 4.0 Visualisations.ipybn
Description:
Important visualization of the data can be seen through this python code
Inputs:
●	drugsComTest_raw.csv
●	drugsComTrain_raw.csv


File name: project 4.1 Sideeffect.ipybn
Description:
The python code extracts data from drugs.com using selenium and beautiful soup
Output : Important(please read this section)
●	Side-effect.csv:  contains the list of side effect(extracted from drugs.com). 
●	side-effect_S.csv:  when the individual words present in the side-effect list is saved and the duplicated words are removed  with all the preprocessing required.
●	side-effec_s.csv : Manually removed words from the (side-effect_S.csv) file to get better results 
●	conditional_probability.csv : this uses (side-effec_s.csv ) file and (Side-effect.csv) to compute how many times the words present in the (side-effec_s.csv ) file is repeated in (Side-effect.csv) file 
 

File name: project 4.2(filtered and n grams).ipybn
Description: 
This is a core file which contains compares words from reviews to words in side- effect library and then join the words that exceeds the threshold probability (0.15). 
Inputs:
●	side-effec_s.csv
●	conditional_probability.csv
output:
●	database.csv:  This is the final file and will be used represent all the required information. Also all the drugs in this file have number of reviews greater than 10.
 
![image](https://user-images.githubusercontent.com/66263773/188257685-cfc06060-d923-4ecb-95c9-6bd7ad06bb75.png)


Deployment:-
File name: Streamlit_Deployment.py
Description: The Python program is used for the purpose of deployment in Streamlit 
Inputs:  database.csv

![image](https://user-images.githubusercontent.com/66263773/188257693-fe1c0f48-7c3b-419d-adaf-9b0b95e2fa43.png)

 

