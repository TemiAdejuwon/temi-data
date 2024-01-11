## Nigerian GDP Analysis

**Project description:** This was a project focused on cleaning and manipulating  Nigerian GDP data


### Dataset used

In this project we will use a dataset from located [here](https://nigerianstat.gov.ng/elibrary/).

 [Nigeria GDP Dataset ](/docs/GDP_rawdata.xlsx)

The Excel file comprises four sheets. Only the first sheet was required for analysis so the efforts in this project are focused on cleaning and manipulating the data on the first sheet. 

### 1. Understanding the GDP dataset 
The dataset shows quarter figures for the years 2020, 2021,2022 for each activity sector and each activity sector group. The gdp is being given at current basic prices and constant basic prices. At constant price is a reference to the real GDP, while at current basic prices is a reference to the nominal GDP. GDP is also recorded for every activity sector.  

<img src="images/excel1.png?raw=true"/>
<img src="images/excel2.png?raw=true"/>

We have about 46 sectors  and 13 groups. Example on Agriculture you have 4 sectors. Crop production, Livestock, Forestry and Fishing. Agriculture, Mining, Manufacturing etc are all activity sectors groups. We can notice this is the same for both Nominal and Real GDP. In the data we can also see we all have Totals for each year based on the quarters  and summation of the GDP along with the net indirects taxes.

Now that we understand our data more we can begin normalizing our data into structured databases format.


### 2. Data Normalization

Normalizing our data means to create a standard format for reporting data, this is known as the development  of clean data to improve integrity 
To normalize our current dataset, we can remove the totals and summation, these can  always be recalculated, also we create proper segments on activity sector and activity sector group and finally categorize the GDP into nominal and real.

Also, I’ll advice to save the file as a new file so that you can also have a copy of your raw dataset 


<img src="images/excel3.png?raw=true"/>


From the images above , you can see we now have 12 columns
- Gdp_type 
- Activity_sector_group
- Activity_sector
- Q1 2020
- Q2 2020
- Q3 2020
- Q4 2020
- Q1 2021
- Q2 2021
- Q3 2021
- Q4 2021
- Q1 2022

In addition to eliminating the total and introducing new columns, we have also modified the quarter columns to incorporate the corresponding year. The data now appears more organized, allowing us to proceed with the transformation using the Power Query Editor.

Additionally, it is crucial to convert your Excel worksheet range into a table before loading it into Power Query.

### 3. Data Cleaning

With our data now organized in a structured format, the next step is to load it into the Power Query for further refinement in our data cleaning process.

The provided image displays the Power Query interface where we will be implementing our transformations. Moving forward, it's essential to identify the specific types of transformations that need to be applied.

<img src="images/excel4.png?raw=true"/>


We will be executing several transformations, including removing the numbers from the activity sector, converting the text to lowercase, pivoting the data, and establishing accurate date formats.
NOTE: Each transformation step undertaken will be documented in the right pane of the editor under "Applied Steps."

<img src="images/excel5.png?raw=true"/>

The transformation process is complete, and we are content with the appearance of our data. We will proceed to close the Power Query editor and load all the implemented changes into a worksheet.

<img src="images/excel6.png?raw=true"/>

The data is now prepared for analysis and visualization.






