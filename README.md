<h1 style="text-align: center; color: blue;">Will a Customer Accept the Coupon?</h1>
<p>This Python application using Jupyter Notebook explores a dataset containing information of ~13,000 people in order to determine which factors make them accept a driving coupon.</p>
<p><a href="https://github.com/Balu-A/AmazonProject/blob/master/AmazonCouponApplication.ipynb" target="_blank">Jupiter Notebook used</a></p>
<p> The current CRISP-DM Process Model for Data Mining (see Figure 1) was followed.</p>
<p align="center">
<img src="images/Figure1_CRISP_DM_Model.jpeg" width="300px" height="300px">
<h4 align="center"> Figure 1</h4>
</p>

<h2>Business Understanding</h2>
The Business task is to identify which factors make a customer accept a coupon delivered over the phone by using python & its libraries in jupyter notebook. This application will use visualizations 
and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

<h2>Data Understanding</h2>
The dataset (coupons.csv) given is in .csv format.It consisted of 26 columns and ~13000 rows as shown below (see Figure 2). The target column is "Y" which is boolean. 
There are only 8 columns that are numerical and the rest are categorical (ordinal and nominal). Columns such as "car", "Bar", "Coffee House", "CarryAway", "Restaurant<20", and 
"Restaurant 20To50" contain a bunch of "NaN" values. Duplicates were also observed. It is thought that in order to provide  more insight into the aforementioned dataset, 
a data preparation, i.e, data cleaning process needs to be done first.
</br>
</br>
<p align="center">
<img src="images/Data_types.png" width="1585px" height="220px">
<h4 align="center"> Figure 2</h4>
</p>


<h2>Data Preparation</h2>
The first step was to drop the null values (see Figure 3), and also make sure that there aren't any duplicates present in the dataset as well. As it is observed in Figure 4, 
all the columns now have same number of rows with no null values.
 
<p align="center">
<img src="images/null-check.png" width="960px" height="275px">
<h4 align="center"> Figure 3</h4>
</p>
 
After cleaning up null values and dupes
<p align="center">
<img src="images/non-nulls.png" width="1278px" height="245px">
<h4 align="center"> Figure 4</h4>
</p>

<h2>Analysis and Visualization of Bar Data</h2>
<h3>Observation 1:</h3> Among the accepted coupons, CoffeeHouse coupons are widely accepted, followed by coupons for cheap restaurants 
<p align="center">
<img src="images/CouponViz.png" width="680px" height="480px">
<h4 align="center"> Figure 5</h4>
</p>

 
<h3>Observation 2:</h3> Among the transmitted Bar coupons, only 41% of the coupons were accepted 

 
<h3>Observation 3:</h3> Among bar-goers, people who frequented bars between 4 and 8 visits per month are more likely to accept the bar coupon. Equally probable are the lot who visited a bar more than 8 times a month 
<p align="center">
<img src="images/Bar_LessThan3_vs_Others.png" width="535px" height="391px">
<h4 align="center"> Figure 6</h4>
</p>

 
<h3>Observation 4:</h3> Bar-goers who are more than 25 yo and who visited a bar more than once a month are more likely to accept a bar coupon than the remaining data set 
<p align="center">
<img src="images/Bar_MoreThan1_25YO_vs_Others.jpg" width="800px" height="453px">
<h4 align="center"> Figure 7</h4>
</p>

 
<h3>Observation 5:</h3> Bar-goers who visited a bar more than once a month, who didn't travel with a kid, and who did work in Farming, Fishing, and Forestry are more likely to accept a bar coupon. This is possibly because those
who work in farming/forestry/fishing may have impeding factors such a work schedule and proximity to a bar 
<p align="center">
<img src="images/Bar_MoreThan1_NoKid_NoFarmvs_Others.jpg" width="957" height="453px">
<h4 align="center"> Figure 8</h4>
</p>


<h3>Overall Hypothesis:</h3> 
<span style="color: red;">If a person is between 25 and 30 years of age and they love going to a bar more than 3 times a month, then there is high likelihood of that person accepting a bar coupon. </span>

<h2>Analysis and Visualization of Cheap Restaurant Data</h2>

<h3>Observation 1:</h3> Of all the distributed cheap restaurant coupons, Unemployed and Student groups are the biggest chunk who accepted the coupon. Those who worked in Farming, Fishing, and Forestry are again the only 
who didn't accept restaurant coupons. This is possibly due to the nature of their work and proximity to a restaurant.
<p align="center">
<img src="images/Coupons_Professions.jpg" width="596px" height="730px">
<h4 align="center"> Figure 8</h4>
</p>
 
<h3>Observation 2:</h3> Among those who accepted the coupon, those who are either single or married to a partner are the biggest recipients of the coupon. Divorcees are least likely to accept a coupon to a cheap 
restaurant. It is possible that Divorcess may accept coupons to a bar.
<p align="center">
<img src="images/Unemployed_Marital_MoreThan4.png" width="1235px" height="600px">
<h4 align="center"> Figure 8</h4>
</p>

<h3>Observation 3:</h3> Also, the unemployed and single lot, when they travel with friend(s) are highly likely to accept a coupon to a cheap restaurant. These are also the people who visit a cheap restaurant more than
4 times a month
<p align="center">/
<img src="images/Unemployed_Unmarried_Various.jpg" width="1267" height="453px">
<h4 align="center"> Figure 8</h4>
</p>

<h3>Observation 4:</h3> What is going on with folks in Farming, Fishing, and Forestry? I wanted to see if this lot accepts any coupon at all and it seems that they do accept carry out/take away coupons. This explains
because of their nature of work and work schedule. Also, their income is under $50K, so presumption is that this lot is frugal.
<p align="center">
<img src="images/FFF_Coupons.jpg" width="737px" height="594px">
<h4 align="center"> Figure 8</h4>
</p>

<h3>Overall Hypothesis:</h3> 
<span style="color: red;">If a person is unemployed and is single or married and they love going to a restaurant more than 3 times a month, then there is high likelihood of that person accepting a coupon to a cheap 
restaurant. </span>

