<h1>Will a Customer Accept the Coupon?</h1>
This python application using jupyter notebook explores a dataset containing information of ~ 13000 people in order to determine which factors make them accept a driving coupon 

[Jupiter Notebook used](https://github.com/Leopard-2019/What-Drives-the-Price-of-a-Car/blob/main/notebook/PracticalApplicationAssignment_11_1-Copy1.ipynb)

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
There are only two more columns numerical: "odometer" and "year", i.e., the rest of the columns were categorical (ordinal and nominal). Consequently, most of the dataset provided will be imbalanced 
before entering the modeling phase. All the columns, but "region", "price", and "state" contain a bunch of "NaN" values. Duplicates were not observed. It is thought that in order to provide  more 
insight into the aforementioned dataset, a data preparation, i.e, data cleaning process needs to be done first.

</br>
</br>
<p align="center">
<img src="images/figure2_data_1.jpeg" width="400px" height="500px">
<h4 align="center"> Figure 2</h4>
</p>

