# Happiness Data Analysis (based on 2015-2019 data)

 ## We conducted data analysis of a feeling of happiness and its relationship with the following factors in 158 countries in 2015 through 2019 :
  
  
### 1. GDP per Capita
### 2. Life Expectancy
### 3. Trust in Government
### 4. Family support
### 5. Freedom
### 6. Generosity

### In this analysis, we took the following path of analysis:

### 1. Exploratory Data Analysis (EDA): Descriptive statistics and distribution of each variable. 
### 2. (EDA) Quick glance of happiness score in top 30 countries from 2015-2019 & Scores of 5 variables in those countries
### 3. Correlation among variables in each year
### 4. Analysis of causal relationships (multiple linear regression analysis)
### 5. Further Exploratory Data Analysis (EDA)

## 1.Exploratory Data Analysis
### Each variable in each year was plotted to take a look at distribution.
![Happiness Score 2015-2019](https://user-images.githubusercontent.com/46631208/115151154-a793e680-a039-11eb-9364-135519430496.png)



![GDP per Capita in 2015-2019](https://user-images.githubusercontent.com/46631208/115151163-b4183f00-a039-11eb-987d-113ff58c8e7c.png)

![Life Expectancy 2015-2019](https://user-images.githubusercontent.com/46631208/115151168-b8445c80-a039-11eb-9f71-9a13ae760d5a.png)

![Trust (Government Curruption) 2015-2019](https://user-images.githubusercontent.com/46631208/115151176-bed2d400-a039-11eb-9ab0-dbf4c4185af7.png)

![Family support in 2015-2019](https://user-images.githubusercontent.com/46631208/115151199-d5792b00-a039-11eb-9f8b-c214ed1d1040.png)

![Generosity 2015-2019](https://user-images.githubusercontent.com/46631208/115151207-dca03900-a039-11eb-8645-82cd1ed22118.png)

### Distribution of each variable shows that these are nicely distributed and can be used for further analysis without a transformation.

## 2. Next, we plotted data points of top 30 happiest countries for all 6 variables (Happiness, GDP per Capita, Family support, Life Expectancy, Trust in government, Generosity)

![Top 30 happiest countries 2015-2019](https://user-images.githubusercontent.com/46631208/115151771-5df8cb00-a03c-11eb-9627-bbccb0568dab.png)

![GDP per Capita in top 30 happiness countries in 2015-2019](https://user-images.githubusercontent.com/46631208/115151780-66510600-a03c-11eb-8b7a-f970e25a2ffb.png)

![Life Expectancy in top 30 happiness countries in 2015-2019](https://user-images.githubusercontent.com/46631208/115151783-6bae5080-a03c-11eb-9290-62be9f248b1d.png)

![Trust in Government in top 30 happiness countries in 2015-2019](https://user-images.githubusercontent.com/46631208/115151789-71a43180-a03c-11eb-81eb-1c797cd019d7.png)

![Family support in top 30 happiness countries in 2015-2019](https://user-images.githubusercontent.com/46631208/115151797-78cb3f80-a03c-11eb-94aa-94a983af2db9.png)

![Generosity in top 30 happiness countries in 2015-2019](https://user-images.githubusercontent.com/46631208/115151804-7e288a00-a03c-11eb-835e-3be6e5cfebba.png)

### Plotting data points of each variable somehow indicates relationships between a feeling of happiness and the other 5 variables. We calculated Pearson correlation coefficient among the variables.


## 3. Correlation Analysis

![Correlation Heatmap 2015](https://user-images.githubusercontent.com/46631208/115151899-ed9e7980-a03c-11eb-93f8-796d0001739f.png)


![Correlation Heatmap 2016](https://user-images.githubusercontent.com/46631208/115151932-145cb000-a03d-11eb-8bec-993ed35c9ff9.png)


![Correlation Heatmap 2017](https://user-images.githubusercontent.com/46631208/115151935-17f03700-a03d-11eb-9979-10862aeaf60d.png)


![Correlation Heatmap 2018](https://user-images.githubusercontent.com/46631208/115151937-19b9fa80-a03d-11eb-8f92-fa7e4dd15455.png)


![Correlation Heatmap 2019](https://user-images.githubusercontent.com/46631208/115151942-1e7eae80-a03d-11eb-8ce5-2b58f2066fdd.png)












