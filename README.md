<h1>Will a Customer Accept the Coupon?</h1>
This python application using jupyter notebook explores a dataset containing information of ~ 13000 people in order to determine which factors make them accept a driving coupon 

[Jupiter Notebook used](https://github.com/Balu-A/AmazonProject/blob/master/AmazonCouponApplication.ipynb)

The current CRISP-DM Process Model for Data Mining (see Figure 1) was followed.

</br>
</br>
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
</br>
</br>
<p align="center">
<img src="images/null-check.png" width="960px" height="275px">
<h4 align="center"> Figure 3</h4>
</p>

</br> 
After cleaning up null values and dupes
<p align="center">
<img src="images/non-nulls.png" width="1278px" height="245px">
<h4 align="center"> Figure 4</h4>
</p>