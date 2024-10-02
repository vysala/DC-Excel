# DC-Excel

-- Webscraping in Excel --

Applied Steps:
 
Get the web data from " https://en.wikipedia.org/wiki/2020_Summer_Olympics_medal_table " 
In Excel , Click Data->Get Data->Select Web -> ' Provide the URL -> Click on Transform Data ( Open the Power Query ) 

**# Check out the 5 basic steps done on this dataset as part of data cleaning: 
**
#Step 0: Rename  NOC column as Country 

****# Step1**:[If the first row is not set as the header go ahead and set it as the header]
1) To make first row as the header 
In the Home ribbon -> check 'Use First row as header '

**#Step2** : Check if any value needs to be replaced
**# Replace the * that appears in the Country Column for the value Japan* . [use replace]. 
    -Right click on the Country Column and select replace value (Replaced * with nothing) 

**#Step3**: Use Fill Down 
**# Go to Transform -> Select Fill ->  fill the null value in the 'Rank' Column with the previous value. For the table from the web, the cell 36 
is merged with the next, as Greece and Uganda shares the same rank. 
Transform->Fill->Down

**#Step 4**: Filter out the last row as it is not required. 

It is similar to specifying a where condition in sql
Select the Rank Column, click on filter symbol and uncheck the Totals(93 entries) 

****#Step 5**: Check the Column Quality indicator.
You can find the column Quality indicator at the top just after the column headers , hover on it to see the quality of data before you starting with data analysis. 
