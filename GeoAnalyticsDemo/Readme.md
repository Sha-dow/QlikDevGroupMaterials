## GeoAnalytics with Advanced Analytics Tutorial

In this tutorial you will go through the following features of Qlik Sense:
* Creating a simple data model using Data Manager
* Creating Master Dimensions and Measures
* Creating drillable GeoAnalytics Map with Area Layer
* Creating a KMeans clustering model using R and presenting this information on map
* Creating an info buble using HTML and on the fly chart generation
* Handling variables 

### Prerequirements
* [Qlik Sense](www.qlik.com)
* Qlik GeoAnalytics
* [R-Studio](https://www.rstudio.com)
* [Qlik Advanced Analytics Extension](https://github.com/qlik-oss/sse-r-plugin)
* [Variable extension](http://branch.qlik.com/#!/project/56728f52d1e497241ae697f8)

### Preparations
* Load datafiles to your computer
  * [Finnish and Swedish community info and Zipcode areas](GeoAnalyticsDemo/Data/DataFiles.zip)

### Step 1: Data Model

* Open Qlik Sense and create new application
* Add Data.qvd, Kuntarajat.qvd and PostalCodes.qvd to application using Data Manager
* You should see 3 bubbles in Data Manager (Image 1)

![Image 1: QVD-files added to Data Manager](https://github.com/Sha-dow/QlikDevGroupMaterials/blob/master/GeoAnalyticsDemo/Images/Step1.png)
*Image 1: QVD-files added to Data Manager*

* Press Magic Wand icon ![](https://github.com/Sha-dow/QlikDevGroupMaterials/blob/master/GeoAnalyticsDemo/Images/Step2.png) on a right hand side to create links between imported tables 

* You should see tables linked together (Image 2)

![Image 2: Files linked together](https://github.com/Sha-dow/QlikDevGroupMaterials/blob/master/GeoAnalyticsDemo/Images/Step3.png)
*Image 3: Files linked together*

* Add paavo_1_he.csv -file to project. This file contains population data from Finnish postal code areas.
* In Add Table -view change Delimiter to Comma, Header Size to 2 and tick Add Fields (Image 3)

![Image 3: Add Table options](https://github.com/Sha-dow/QlikDevGroupMaterials/blob/master/GeoAnalyticsDemo/Images/Step4.png)
*Image 4: Add Table options*
