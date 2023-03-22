# MATLAB-Data-Plotting-Tutorial
Given an Excel file, we will extract data and plot a simple graph with a choice of markers.
This tutorial is beginner friendly, but is dependent on the user downloading MATLAB beforehand and having a license which done by using a college email and registering an account.

In this tutorial we will use an Excel data file that is attached to this repository called boston_data.xls which contains example time, air temperature, wind speed, dewpoint, etc. data. 

However we need to convert the Excel file into a .txt file in order to make the data readable for the program. To do this we would open up the boston_data.xls file on Excel, select file on the top right of the screen, select save as, select tab delimited file, and save the file into a separate project folder that will hold the additional MATLAB files. 

Nice! Now we can open up MATLAB and create a new script which is a new file where you would be writing out all your code! Let's start with naming the script by using double percentage signs (%%) which will allow us to comment and create a new header. Then let's add in the owner of the file using one perventage sign (%) which is usually used as in-line comments:  

<img width="714" alt="Screenshot 2023-03-21 at 6 08 04 PM" src="https://user-images.githubusercontent.com/110073567/226752658-51795d6f-66aa-4127-a1cd-46676e703a2f.png">

After creating the comments let's set up our input codes:

<img width="716" alt="Screenshot 2023-03-21 at 6 08 56 PM" src="https://user-images.githubusercontent.com/110073567/226752812-7e01f6b2-0870-4cf7-8ad1-bc126549d8ca.png">

Clear and load are both commands of MATLAB. Clear removes any and all variables existing in the workspace to the right:

<img width="309" alt="Screenshot 2023-03-21 at 6 12 11 PM" src="https://user-images.githubusercontent.com/110073567/226753410-343ebe9a-107e-4950-bcc2-df2512aa1746.png">

When setting up variable for data in certain columns, we would use the format of variable = dataVariable(:,1); where the (:,1) represents the data in the first column of the .txt file. Referencing data columns as variables makes it easier for the users to call on that specific data set later. 

```Matlab
time = b(:,1); %set a variable for time by using the data's first column
windspeed = b(:,2); %set a variable for windspeed by using the data's second column
tair = b(:,3); %set a variable for air temperature by using the data's third column
td = b(:,4); %set a variable for dew point by using the data's fourth column
pressure = b(:,5); %set a variable for air pressure by using the data's fifth column 
```
