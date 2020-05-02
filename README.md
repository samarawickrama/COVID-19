# A Framework for Rapid Prototyping Data-Science Modelling of COVID-19 Data with Countries' Statistics

## Introduction

COVID-19 became a global pandemic which has impacted human life in every aspect. Because the infection is fast spreading and endangering the human life, immediate actions need to be taken to prevent the disease in community level. By now every country has faced COVID-19 pandemic and their statistics show greater diversities. It is not quite obvious what the qualities, factors and strategies should be to focus on short-term and long-term, to   effectively face COVID-19 and similar pandemics [1, 2].

Since this is a multidimensional challenge going beyond simple imagination, data science is an effective strategy to understand the  patterns and trends in the data related to COVID-19. While data science is an effective technique to uncover insights, wide community and professionals currently rely on open visualization frameworks which mostly cover descriptive analysis techniques. If an user-friendly open data-science framework is available, subject matter experts (SMEs) can effectively adopt and effectively interpret the insights to social and human benefits [3]. 

This is a framework for rapid prototyping data-Science modelling of COVID-19 data with countries' statistics. This will help to link big datasets with COVID-19 data followed by applying advanced modelling techniques  based on machine learning. This contributes to democratizing COVID-19 related data science and analytics and promote data driven decision making and innovations.

## Adopt the Framework

This framework is developed using Jupyter notebook and Python libraries. Users can install Jupyter notebook easily by installing Anaconda. Any platform which supports Jupyter notebook can be used (e.g., AWS Sagemaker). The Jupyter notebook project is available in Github.

## Datasets

To demonstrate the framework, two widely used datasets were used. They are: 

1) Johns Hopkins University (JHU) and Worldometers.info open data for COVID-19 statistics of countries
2) World Bank open data for countries data and statistics

The data is available as Python libraries. Users can access this data by importing the libraries. The libraries have appropriate APIs to access the data.

Following are important references to the used libraries.

However, users do not want to limit to above data or libraries as many data sources are available to easily integrate with this framework.

## Methodology

The platform is demonstrated using Johns Hopkins University (JHU) and Worldometers.info open data for COVID-19 [4] and World Bank open data for countries [5]. The data is imported to the framework using published Python libraries (as given in the above section).

In Johns Hopkins University (JHU) and Worldometers.info open data for COVID-19, the countries' statistics related to confirmed, active, recovered and deaths cases are provided together with updated date.

On the other hand,  World Bank open data for countries is a general and versatile dateset which provides diversified statistics related to multiple topics. It is not developed focusing COVID-19 crisis. This data-set has countries' statistics related to the following 21 topics.

Jupyter notebook with Python help to explore and prepare data efficiently. Throughout the framework, data is handled as Pandas data-frames. Python matplotlib and seaborn libraries are used as required to visualize and explore the data. Since World-Bank dataset has many features, exploratory analysis techniques are required to effectively prepare data for accurate modelling.

![Image description]https://drive.google.com/file/d/1v9rawRq0BqbbzVh2qoUJ3TsP_3dK0P3B/view?usp=sharing

The framework adopted LightGBM gradient-boosting decision-tree based machine learning algorithm to design and implement classification and regression models. This algorithm is being used quite effectively in industry to model structured data. It has following advantages [6]:
 - Faster training speed and higher efficiency,
 - Lower memory usage,
 - Better accuracy,
 - Support of parallel and GPU learning
 - Capable of handling large-scale data.

Once the model is trained, the framework then facilitates important-feature analysis based on high-ranked features of the LightGBM algorithm. This includes adaptation of SHAP (SHapley Additive exPlanations) library which enables to evaluate the trained machine-learning models using the incorporated features using a game theoretic approach [7]. This enables reasoning and prescription related to the hypothesis. The framework also facilitates evaluation of the training and testing performances. The important-feature analysis and performance analysis stages are important to optimize the model by tuning and retraining the models.

## Conclusion

Many research data has been published related to COVID-19 and it is required for fast analysis of these data and communicate the insights (i.e., prescriptive analytics) to community to improve the health and wellbeing. Because of the high dimensionality of the data, data-science capabilities around this COVID-19 data analysis need to be enhanced. This proposed framework enables rapid prototyping of data-science modelling of COVID-19 data with countries statistics which effectively democratize COVID-19 related data science and analytics.

## Future Work

There are many datasets emerging which will enhance the knowledge if they are properly analyzed in unified way. Following datasets are being planned to be incorporated with the proposed framework.

Further, we are planning to analyse the data in suburb level by incorporating the census data of countries.

## References

[1] Xu, B., Gutierrez, B., Mekaru, S. et al. Epidemiological data from the COVID-19 outbreak, real-time case information. Sci Data 7, 106 (2020). https://doi.org/10.1038/s41597-020-0448-0

[2] Dong, E., Du, H., & Gardner, L. (2020). An interactive web-based dashboard to track COVID-19 in real-time. The Lancet Infectious Diseases. https://doi.org/10.1016/S1473-3099(20)30120-1

[3] Callaghan S. COVID-19 Is a Data Science Issue. Patterns. 2020 Apr 7:100022. doi: 10.1016/j.patter.2020.100022. Epub ahead of print. PMCID: PMC7144860.
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7144860/

[4] Dataset provided by Johns Hopkins university and worldometers.info
https://ahmednafies.github.io/covid/

[5] World Bank Open Data
https://data.worldbank.org/

[6] LightGBM, Light Gradient Boosting Machine
https://github.com/microsoft/LightGBM

[7] SHAP (SHapley Additive exPlanations)
https://github.com/slundberg/shap
