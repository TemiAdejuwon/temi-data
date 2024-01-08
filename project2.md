## King County Housing Sales

**Project description:** This project was done to analyze the Nigerian GDP


### Dataset used

In this project we will use a dataset from located [here](https://nigerianstat.gov.ng/elibrary/).

 [Nigeria GDP Dataset ](/docs/HouseData.xlsx)

The Excel file comprises four sheets. Only the first sheet was required for analysis so the efforts in this project are focused on cleaning and manipulating the data on the first sheet. 

### 1. Understanding the GDP dataset 
The dataset shows quarter figures for the years 2020, 2021,2022 for each activity sector and each activity sector group. The gdp is being given at current basic prices and constant basic prices. At constant price is reference to the real GDP, while at current basic prices is a reference to the nominal GDP. GDP is also recorded for every activity sector. 

<img src="images/excel1.png?raw=true"/>
<img src="images/excel2.png?raw=true"/>

We have about 46 sectors  and 13 groups. Example on Agriculture you have 4 sectors. Crop production, Livestock, Forestry and Fishing. Agriculture, Mining, Manufacturing etc are all activity sectors groups. We can notice this is the same for both Nominal and Real GDP. In the data we can also see we all have Totals for each year based on the quarters  and summation of the GDP along with the net indirects taxes.

Now that we understand our data more we can begin normalizing our data into structured databases format.

### 2. Data Normalization

Normalizing our data means to create a standard format for reporting data, this is known as the development  of clean data to improve integrity 
To normalize our current dataset, we can remove the  Totals and summarization, these can  always be recalculated, also we create proper segments on activity sector and activity sector group and finally categorize the GDP into nominal and real.

Also, I’ll advice to save the file as a new file so that you can also have a copy of your raw dataset 

<img src="images/excel3.png?raw=true"/>
<img src="images/excel4.png?raw=true"/>

From the images above , you can see we now have 12 columns
-Gdp_type 
-Activity_sector_group
-Activity_sector
-Q1 2020
-Q2 2020
-Q3 2020
-Q4 2020
-Q1 2021
-Q2 2021
-Q3 2021
-Q4 2021
-Q1 2022

Aside from removing the total and creating new columns, we also edited the quarter columns to include the year.
As you can see our data is looking a lot better and easier to understand now move on to data cleaning using power query editor. 

Also, it important to note to convert your excel worksheet for range to Table before loading into power query



### 3. Data Cleaning


### 4. Provide a basis for further data collection through surveys or experiments

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
