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

### All data process and statistical analysis were conducted by Python.

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

### 2015 data correlation
![Correlation Heatmap 2015](https://user-images.githubusercontent.com/46631208/115151899-ed9e7980-a03c-11eb-93f8-796d0001739f.png)

### 2016 data correlation
![Correlation Heatmap 2016](https://user-images.githubusercontent.com/46631208/115151932-145cb000-a03d-11eb-8bec-993ed35c9ff9.png)

### 2017 data correlation
![Correlation Heatmap 2017](https://user-images.githubusercontent.com/46631208/115151935-17f03700-a03d-11eb-9979-10862aeaf60d.png)

### 2018 data corelation
![Correlation Heatmap 2018](https://user-images.githubusercontent.com/46631208/115151937-19b9fa80-a03d-11eb-8f92-fa7e4dd15455.png)

### 2019 data correlation
![Correlation Heatmap 2019](https://user-images.githubusercontent.com/46631208/115151942-1e7eae80-a03d-11eb-8ce5-2b58f2066fdd.png)

### We would like to take a closer look at relationships of those variables.

### 2015 data pairplot
![pairplot2015](https://user-images.githubusercontent.com/46631208/115152077-ab296c80-a03d-11eb-922c-511b2bb4a21b.png)

### 2016 data pairplot
![pairplot2016](https://user-images.githubusercontent.com/46631208/115152081-af558a00-a03d-11eb-9a88-a20204f818b0.png)

### 2017 data pairplot
![pairplot2017](https://user-images.githubusercontent.com/46631208/115152087-b1b7e400-a03d-11eb-87c9-1725394c05e8.png)

### 2018 data pairplot
![pairplot2018](https://user-images.githubusercontent.com/46631208/115152092-b41a3e00-a03d-11eb-95f0-a737ee1ee7ea.png)

### 2019 data pairplot
![pairplot2019](https://user-images.githubusercontent.com/46631208/115152095-b9778880-a03d-11eb-9d98-51df008bd95f.png)

### The correlation analysis revealed a strong relationship among Happiness, GDP per Capita, Family support, and Life Expectancy.

## 4. Causal Relationships (Multiple Linear Regression Analysis)
### Based on the relationships among variables we explored how well we can predict the happiness score in each country from the other 5 variables. The correlation analysis leads us to assume strong influences from GDP per Capita, Life Expectancy, and Family Support as well as intermediate influence from Freedom. 

![multiple_regression_result](https://user-images.githubusercontent.com/46631208/115152618-c9906780-a03f-11eb-93d2-149cde927d5b.PNG)


### Multiple linear regression analysis found that GDP per Capita and the life expectancy influence a feeling of happiness as expected. However, the family support has a relatively small influence on the happiness (coefficient = 0.58, p<.01). Since the family support is highly correlated to a high income and longer life, these factors might enable people in those countries to support each other among family. In other words, higher income and longer life might make it easier to support other family members.

### Despite a relatively low correlation coefficient with the happiness (r=0.54 to 0.57), the freedom has a highest impact on the happiness score (coefficient = 1.705, p<.01).

## 5. Further Exploratory Data Analysis
### Top 30 happiness countries data plot shows that many of them are Westernized countries (Switzerland, Iceland, Denmark, Norway, Canada, Finland, Netherland, and Sweden, etc.).
### We will colorcode each country by the level of happiness to see if the regional tendency of happiness level.

### Happiness level mapping 2015
![happiness_score_map_2015](https://user-images.githubusercontent.com/46631208/115152835-d95c7b80-a040-11eb-8b24-d44202612e52.PNG)


### Happiness level mapping 2016
![happiness_score_map_2016](https://user-images.githubusercontent.com/46631208/115152848-ee390f00-a040-11eb-8116-fd15d6f4af24.PNG)

### Happiness level mapping 2017
![happiness_score_map_2017](https://user-images.githubusercontent.com/46631208/115152864-fdb85800-a040-11eb-81e5-ec020351042a.PNG)

### Happiness level mapping 2018
![happiness_score_map_2018](https://user-images.githubusercontent.com/46631208/115152874-0872ed00-a041-11eb-98e3-92f4f41c2099.PNG)

### Happiness level mapping 2019
![happiness_score_map_2019](https://user-images.githubusercontent.com/46631208/115152881-132d8200-a041-11eb-9614-1b7e504c75bd.PNG)

### The world map with coloring based on the happiness level shows that western countries are highly likely to be rated for one of the happiest countries. The other countries are rated low happiness. However, we need to be careful to conclude that the happiness level or happiness ranking shows how good the happiest people are. A feeling of happiness is just one of many indicators to measure quality of their lives.


