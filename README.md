# Amazon_Vine_Analysis

## Overview
In this module we utilized Google Colab, Amazon AWS and PG Admin to process large amounts of data (Big Data) that exceed the capacity of operational databases. Big data contains four categories, these are: 
 - Volume
 - Velocity
 - Variety
 - Veracity

In this scenario we are tasked with analizing mazon Product reviews written by members of the paid Amazon Vine program. 

### *Deliverable #1*

Create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasetsLinks to an external site., and extract the dataset into a DataFrame transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, you'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

## DataBase Created in AWS / Amazon RDS  

![image](https://user-images.githubusercontent.com/104601282/197328841-6835c908-2cd2-44bf-b5a9-169329712caa.png)


### Tables Created in Google Colab 

*Customer Table & Product Table below*

![image](https://user-images.githubusercontent.com/104601282/197328569-76e7006f-6333-4b59-8584-b646d01ed260.png)


*Review Table and Vine Table Below* 

![image](https://user-images.githubusercontent.com/104601282/197328650-e40955d5-334c-4049-bb18-de8484fd7e10.png)
![image](https://user-images.githubusercontent.com/104601282/197328705-c69c7729-fc3c-41e8-9f78-7df3de6e9d4b.png)

### Tables Created in PG Admin 

![image](https://user-images.githubusercontent.com/104601282/197328933-fdcfbed9-ea4d-4335-8000-762f669ebee7.png)


### *Deliverable #2*
To Complete this deliverable I chose PG Admin to conduct my analysis. The objective of this deliverable is to determine if having a paid Vine review makes a difference in the percentage of 5-star reviews. To complete this deliverable the requirements are as follows: 

   1. Create a new table to retrieve all rows where total votes re => 20.
 Included above the table below are the parameters used to generate the data. 
 ![image](https://user-images.githubusercontent.com/104601282/197329978-1a5c84b5-0265-446e-b12d-8d39d8eb62d2.png)

   2. Filter the new DataFrame or table created in Step 1 and create a new DataFrame or table to retrieve all the rows where the number of helpful_votes divided by total_votes is equal to or greater than 50%. Included above the table below are the parameters used to generate the data. 
![image](https://user-images.githubusercontent.com/104601282/197330047-8d0fb570-7763-41cf-ad95-48ee7f6863aa.png)

   3. Filter the DataFrame or table created in Step 2, and create a new DataFrame or table that retrieves all the rows where a review was written as part of the Vine program paid or unpaid. Included above the table below are the parameters used to generate the data. 
![image](https://user-images.githubusercontent.com/104601282/197330069-e9051e4e-2774-4abf-8f56-18f07853b12b.png)

  
   4. Determine the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of review (paid vs unpaid). 
   
      - Total Number of reviews: 2,302,401
      - ![image](https://user-images.githubusercontent.com/104601282/197330927-ea64ec34-4b4c-4b92-ac0a-4ce8971b11ae.png)
      - Five star Rating: 1,434,884
      - Five Star reviews paid vs unpaid 
      - ![image](https://user-images.githubusercontent.com/104601282/197331976-121bb724-476d-4bbf-8f18-2612a7eda16d.png)

## Findings

Based on the data analysis the total reviews recieved where 2302401, 62%  of all the reviews recieved a five (5) star raiting. 
When we compare the paid services makes up less than 1% of the five (5)stars reviews. Non paid reiewers make up 99.88% of the five (5)star reviews. My determination is that there is no higher rating for paid service. 











