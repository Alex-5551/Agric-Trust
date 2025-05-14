
# AgriConnect: A data driven solution to enable young farmers access loan

This project focuses on helping young agripreneurs in Nigeria obtain access to affordable finance by building an app that banks, investors, or grant bodies could trust to fund young farmers.



## Dataset
The dataset used in this project was sourced from the EFInA 2023 Access to Finance (A2F) Survey.
https://efina.org.ng/our-work/research/

However, the dataset was subsetted to youths from age 18 to 25 and also relevant columns were choosen. 
Here is the subset of the dataset used to train the ML model. https://github.com/Alex-5551/Agric-Trust/blob/main/Agri_data.csv



## Python file
https://github.com/Alex-5551/Agric-Trust/blob/main/Agriconnect.ipynb

Explore this file to gain insights into the data cleaning process, visulizations and ML model built.
## Method
The data which is a survey response had 28392 rows and 1613 columns. 

This was reduced to 1055 rows and 29 columns by dropping missing values, subsetting the age columns to individuals from 18 to 25, and then selecting columns that impacts a farmers creditworthiness, such as Average personal income, tax clearance certificate, credit history, education, assets etc. 

First, Kmeans clustering was utilized to cluster the young farmers into two(high creditworthiness and low creditworthiness), after which classification models was used to predict the cluster a farmer fell into.

Two classification model, Random Forest and Gradient boosting was trained. Both gave an acurracy of 1 and also a precision of 1. This means both model was able to correctly predict farmers in both clusters.





## Output
Random forest classifier was able to predict 175 out 175 not creditworthy farmers and 36 out of 36 creditworthy farmers.

The model was used to build a web app to enable banks identify creditworthy farmers who can be trusted with funds.

Feel free to explore the app
https://hackathon-bwcuthflmfynjetsfrmpgt.streamlit.app/

## Conclusion
Key findings from data exploration

1. only 1.9% of the sample youths had tax clearnce certificate and Local Government rates and tax invoice

2. 97.8% of youths don't have insurance

3. 57.5% of the youths are financillay coping

4. 43.8% of the youths have a manageable amount of debt

These findings help explain why younger farmers may face challenges in being considered creditworthy for loans.
