# 711-Stores-Macrospace-Optimization

Analysis of occupied spaces of the beverages products categories in 711 stores in Phillipines. The aim of the project was determinated what would be the best distribution of products in all the stores to optimize the sales. For this purpuse, we analyzed data of millions of transactions (+ 10 GB) in all stores over the past 6 months. Data is stored in a Amazon Redshift Warehouse.

The process begins with the data preparation. For our purpouse we are working with data of 5 beverages categories:
Category 21: Juices and Teas
Category 24: Softdrinks
Category 27: Bottle Water
Category 31: Dairy
Category 32: Beer

Objectives and tasks:
1.	Clean and standarize Dataset
2.	Calculate key indicators: Daily Sales and Daily Sales/Width
3.  Normalized Indicator in order to compare big stores with small stores
4.	Create Exponential math model for the Daily Sales
5.	Calculate optimized space by category by store

Software: 1- Python/  2- PostgreSQL  /  3- Power BI

Chart Trend :Total Sales by Category 
<img
  src="/Images/Salesbymonth.JPG"
  alt="Salesbymonth"
  title="Salesbymonth"
  style="display: inline-block; margin: 0 auto; max-width: 200px">

Transaction data is cleaning and then merged with data of width shelfs and planograms. The idea is , first, to calculate the daily sales by store in each category. Given that we look for optimized the space use in each store, we need to calculate a new indicator, indicator DailySales/Width, where Width is the linear space occupied by that category.  To built the math exponential model, the average of the DailySales/Width value is calculated , and Width 






  
 <img
  src="/Images/dailysalesnormalized.JPG"
  alt="dailysalesnormalized"
  title="dailysalesnormalized"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
  
 <img
  src="/Images/exponentialcurve.JPG"
  alt="exponentialcurve"
  title="exponentialcurve"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
