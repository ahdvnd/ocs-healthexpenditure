# OpenCaseStudies

This case study is part of the [OpenCaseStudies]() project. This work is licensed under the Creative Commons Attribution-NonCommercial 3.0 ([CC BY-NC 3.0](https://creativecommons.org/licenses/by-nc/3.0/us/)) United States License.

The libraries used in this study are `library(datasets)`, `library(tidyr)`, `library(dplyr)`, `ggplot2`, and `ggrepel`. In order to run this code please ensure you have these packages installed.

### Exploring Health Expenditure using State-level data 

Health policy in the Staes is complicated, and several forms of healthcare 
coverage existed in the United States of America, including both federal goverment-led 
healthcare policy, and private insurance company. Before making any inference about 
the relationship between health condition and health policy, it is important for us to 
have a general idea about healthcare economics in the States. Thus, We are interested in 
getting sense of the health expenditure, including healthcare coverage and 
healthcare spending, across States.  

### Motivating question

1. Is there a relationship between healthcare coverage and healthcare spending in the United States?   
2. How does the spending distribution change across geographic regions in the Unied States?  
3. Does the relationship between healthcare coverage and healthcare spending in the United States change from 2013 to 2014?  

### Data

The data for this demonstration come from the [Henry J Kaiser Family Foundation (KFF)](https://www.kff.org). 

* [Health Insurance Coverage of the Total Population](https://www.kff.org/other/state-indicator/total-population/) - Includes years 2013-2016
* [Health Care Expenditures by State of Residence (in millions)](https://www.kff.org/other/state-indicator/health-care-expenditures-by-state-of-residence-in-millions/) - Includes years 1991-2014
 
For learning purpose, data have been downloaded, and relative route is used for this demonstration. 
(Note: If students are not familiar with relative route, it will be helpful to briefly introduce 
the idea for absolute route and relative route.)

We also introduce `library(datasets)` for States information.

### Data Import  
We use the R package `library(readr)` for data import in this tutorial.  

### Data wrangling 
Two R package `library(tidyr)`, `library(dplyr)` are used for data wrangling in this tutorial.  

We explain what tidy data is, and further introduce the concepts of "wide format" 
and "long format." We also demonstrate how to convert from one format to the other using 
`gather()` and `spread()`.

We also demonstrate some other useful functions for data wrangling, including 
selecting columns using `select()`, 
Selecting rows using `filter()`, 
arranging or re-orderomg rows using `arrange()`, 
joining two datasets using `join()`, 
adding columns using `mutate()`, 
creating summaries of columns using `summarise()`, 
and grouping operations using `group_by()`. 


### Data exploration (exploratory analysis)   
For exploratory analysis, we use data visulization for exploratory analysis. `ggplot2` is the R package 
we demonstrate in this tutorial. 

We explain how to create plots using `ggplot()` with basic syntax for `ggplot2`. 
We also demonstrate how to create scatter plots using `geom_point()`,
how to add layers of text using `geom_text()`, 
how to facet across a variable using `facet_wrap()`, 
how to create boxplots using `geom_boxplot()`, 
and how to facet by two variables using `facet_grid`. 


### Summary   

The total healthcare expenditure is associated with 
the population. To make a fair comparison, 
we create "healthcare expenditure per capita." 
Further, the exploratory analysis via data visualization showed 
higher speding in healthcare per capita 
is positively associated with higher 
employer coverage proportion and is 
negatively associated with the porportion 
of uninsured population across the States. 

### Notes for instructors  
1. The objective of this tutorial is for student to get familiar with 
important skills in data science, including data import (`readr`), 
data wrangling (`dplyr`) , and data visualization (`ggplot2`) .    
2. This material is designed for 4.5 teaching hours. (One potential way 
to teach this tutorial is to divide the material into three 1.5 hour sessions. The 
first session focuses on data import, the second session focuses on data 
wrangling, and the third portion focuses on visualization.)    
3. The session starting with (*) can be made as exercise for students' practice.   
