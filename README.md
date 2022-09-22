![HenryLogo](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fpostandparcel.info%2Fwp-content%2Fuploads%2F2012%2F10%2Fdpd-parcel-delivery.jpg&f=1&nofb=1)

# Datathon

## Logistics World Trade

Logistics is a vital market in the globalized world and it connects the world where we live. Coordinating the transport of the entire supply chain from where goods are produced until they reach the end customer is a complex task, which must be planned and executed in the most efficient way for the operation of trade to succeed, both local and global.. 

Thanks to new tools such as the use of GPS, digital records of input and output of distribution centers, and different ways to transport a package by land, sea, and air, in addition to IoT tools throughout the supply and production chain, it is possible to accumulate a lot of data, which can be analyzed to optimize logistics processes.

### Problem description

We are part of a logistics team company that works for an important E-Commerce platform, and our team leader gives us the task of implementing a machine learning model that allows us to predict if a shipment will arrive on time or not. According to the information from the dataset, the company will be able to pay attention and follow up those shipments that may cause problems.

### Metrica to use

$$ Recall=\frac{TP}{TP+FN}$$
siendo $TP$ los verdaderos positivos, $TN$ verdaderos negativos y $FN$ los falsos negativos.

### A dataset has been provided..

Training and test datasets:
- 'E-Commerce_train.xlsx', con 8998 observaciones y 12 dimensiones, incluyendo información sobre si el envío llegó a tiempo o no en el momento del registro. 
- 'E-Commerce_test.xlsx', con 2000 observaciones y 11 dimensiones, sin incluir información sobre si el envío llegó a tiempo o no en el momento del registro.

### Dimensions Description 

- ID: order record identifiern (int).
- Warehouse_block: Distribution warehouse where the order came from (A,B,C,D,E,F).
- Mode_of_Shipment: Ways of transport (Flight, Road, Ship).
- Customer_care_calls: Number of customer service calls for that order. (int values from 2 to 7)
- Customer_rating: Customer Score (Int values from 1 to 5).
- Cost_of_the_Product: Sale price (int).
- Prior_purchases: Number of previous purchases made by the customer (int value from 2 to 10).
- Product_importance: Importance of the product (low, medium, high).
- Gender: Male or female classes only (F, M).
- Discount_offered: Percentage discount offered for that purchase (int value from 1 to 65):
- Weight_in_gms: Weight of the order package, in grams (int).
- Reached.on.Time_Y.N: information about the arrival of the package at its destination (1 if it arrived on time, 0 if it did not arrive on time).

## How to run the code?

* You'll need to fork and clone the repo.
* Create a env with `python3 -m venv ./venv` we also can use conda [conda](https://docs.conda.io/en/latest/). and them let's install the requirements as follows `pip install -r requeriments/dev.txt`.
* To activate venv `source venv/bin/activate`.
* Run jupyter `jupyter-notebook`.
* To deactivate `deactivate`.

## Files Intro

* Datasets: Two \*.xlsx files where the data came from.
* Datawehouse: A set of parquet files (training, validation, and testing) inputs and targets that have been cleaned and are ready to use in any ML model.
* requirements: A set of common, development, and production modules that are required at each stage of the product. 
* EDA.ipynb is made for exploratory data analysis. Each time we run it, we will be exporting an eda_basics_features.joblib with all the data ready to use in the models. 
* The models directory has the machine learning models that would be applicable.

### + Info
* [How to create a virtual enviroment in python](https://www.machinelearningplus.com/deployment/conda-create-environment-and-everything-you-need-to-know-to-manage-conda-virtual-environment/)
* [How to load more than 100mb and csv files to Git LFS](https://stackoverflow.com/questions/33330771/git-lfs-this-exceeds-githubs-file-size-limit-of-100-00-mb)
* [How to install Git LFS to ubuntu](https://askubuntu.com/questions/799341/how-to-install-git-lfs-on-ubuntu-16-04)

<img src = "https://user-images.githubusercontent.com/96025598/188937586-28575753-fbd6-42de-beca-81ae35b659e0.gif" height = 300>


