
# Alberghi Classification


## Exploratory Data Analysis + Data Visualization + Modelling 

### 1 - Abstract

In this project I made Exploratory Data Analysis, Data Visualisation and lastly Modelling which I did with 9 different models. In Exploratory Data Analysis I cleaned irrelevant data,NaN values and change data types for easiness. In second part, I would like to show data in plots.Such as, number of places according to their types and according to province. Later these processes I looked Pearson Correlation and Spearman Correlation which they gave very similar result as expected. Before modelling I prepared data training and testing. My testing size is __0.33__. Then I applied for each model, the algorithms I used for these project are Logistic Regression, K Neighbors Classification, Decision Tree Classification, Random Forest Classification, AdaBoost Classification, Gradient Boosting Classification, XGB Classification, ExtraTrees Classification, Bagging Classification. Finally, Random Forest Classifier gives the best result but tuning with algorithms or cleaning the data more(I believe it will decrease the size of dataset alot) can be effective.

### 2 - Data

Dataset contains 6775 rows and 25 columns.
Description and Type of Each Column;

* __ID                       *int64*__   - id
* __PROVINCIA               *object*__   - id of state
* __COMUNE                  *object*__   - name of city
* __LOCALITA                *object*__   - name of town
* __CAMERE                   *int64*__   - number or rooms
* __SUITE                    *int64*__   - number of suites
* __LETTI                    *int64*__   - number of beds
* __BAGNI                    *int64*__   - number of bathrooms
* __PRIMA_COLAZIONE          *int64*__   - breakfast included or not
* __IN_ABITATO             *float64*__   - building or not
* __SUL_LAGO               *float64*__   - close to lake or not
* __VICINO_ELIPORTO        *float64*__   - close to heliport or not
* __VICINO_AEREOPORTO      *float64*__   - close to airport or not
* __ZONA_CENTRALE          *float64*__   - in the central or not
* __VICINO_IMP_RISALITA    *float64*__   -
* __ZONA_PERIFERICA        *float64*__   - suburb or not
* __ZONA_STAZIONE_FS       *float64*__   - close to station or not
* __ATTREZZATURE_VARIE      *object*__   - equipment types( elevator, park, restaurants etc.)
* __CARTE_ACCETTATE         *object*__   - accepted credit cards (visa,mastercard etc.)
* __LINGUE_PARLATE          *object*__   - spoken languages by host or hotel
* __SPORT                   *object*__   - sport options (football, table tennis etc.)
* __CONGRESSI               *object*__   - congress room(s)
* __LATITUDINE             *float64*__   - latitude
* __LONGITUDINE            *float64*__   - longitude
* __OUTPUT                  *object*__   - types of places

### 3 - Exploratory Data Analysis

Firslty, I checked data types and number of Nan in each columns. Later this process I decided which columns I will delete and which rows should I delete. So I deleted *LOCALITA - SPORT - CONGRESSI - LATITUDINE - LONGITIDUNE* columns and I deleted in NaN rows in *IN_ABITATO -SUL_LAGO - VICINO_ELIPORTO - VICINO_AEREOPORTO - ZONA_CENTRALE - VICINO_IMP_RISALITA - ZONA_PERIFERICA - ZONA_STAZIONE_FS* columns. But I keep 3 columns which contains very high number of NaN values because data they contains could be helpful for future works. 

### 4 - Data Visualization

<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/numberofplaces.png">
</p>
<p align="center">
   <b>Number of Places According to Their Types</b>
</p>

<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/2classificationreport.png">
</p>
<p align="center">
   <b>K Neighbors Classification</b>
</p>


### 5 - Modelling 

* __5.1 - Logistic Regression__

is used to predict the categorical dependent variable using a given set of independent variables. 
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/1classificationreport.png">
</p>
<p align="center">
   <b>Logistic Regression</b>
</p>

* __5.2 - K Neighbors Classification__

non-parametric classification method.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/2classificationreport.png">
</p>
<p align="center">
   <b>K Neighbors Classification</b>
</p>

* __5.3 Decision Tree Classification__

breaks the data smaller subsets in form of tree structure
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/3classificationreport.png">
</p>
<p align="center">
   <b>Decision Tree Classification</b>
</p>

* __5.4 - Random Forest Classification__

consist many decision tree but using bagging and randomness. then look at average/voting and gives the result.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/4classificationreport.png">
</p>
<p align="center">
   <b>Random Forest Classification</b>
</p>

* __5.5 - AdaBoost Classification__

is an meta-estimator, that begins by fitting a classifier on the original dataset and then fits additional copies of the classifier on the same dataset.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/5classificationreport.png">
</p>
<p align="center">
   <b>AdaBoost Classification</b>
</p>

* __5.6 - Gradient Boosting Classification__

combine weak learning models to create strong model.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/6classificationreport.png">
</p>
<p align="center">
   <b>Gradient Boosting Classification</b>
</p>

* __5.7 - XGB Classification__

implementation of gradient boosted decision trees but more effective in performance.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/7classificationreport.png">
</p>
<p align="center">
   <b>XGB Classification</b>
</p>

* __5.8 - ExtraTrees Classification__

implements a meta-estimator which fits number of random decision trees on various subsets of dataset and it uses average/voting to improve prediction.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/8classificationreport.png">
</p>
<p align="center">
   <b>ExtraTrees Classification</b>
</p>

* __5.9 - Bagging Classification__

an ensemble meta-estimator that fits base classifiers each on random subsets of the original dataset and then aggregate their individual predictions  to form a final prediction.
<p align="center">
  <img width="500" height="350" src="https://github.com/HalukSumen/AlberghiClassification/blob/main/images/9classificationreport.png">
</p>
<p align="center">
   <b>Bagging Classification</b>
</p>

### 6 - Result & Future Work

* __Logistic Regression Score:__ 0.6460699681962744
* __K Neighbors Classifier Score:__ 0.6338028169014085
* __DecisionTree Classifier Score:__ 0.8391640163562017
* __Random Forest Classifier Score:__ 0.8727850976828714
* __AdaBoost Classifier Score:__ 0.5483870967741935
* __Gradient Boosting Classifier Score:__ 0.8714220808723308
* __XGB Classifier Score:__ 0.7878237164925034
* __ExtraTree Classifier Score:__ 0.8632439800090868
* __Bagging Classifier Score:__ 0.8514311676510677

According the scores,Random Forest Classifier gives best result with __0.872785__. Also Gradient Boosting is gives very close to Random Forest Classifier with __0.871422__, and finally AdaBoost is give the worst performance with __0.548387__. In the end Random Forest Classifier gives the best result but maybe tuning with XGB increase its score.  
