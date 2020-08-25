# Instacart-Adoption

## Executive Summary
The COVID-19 global pandemic caused a shock to the world. This impact extends from the frontlines of a battle for global health to daily activities that were formerly taken for granted. In particular, the subsequent policies and self-isolating measures taken by the vast population in the face of COVID-19 brought about an unprecedented change in consumer behavior and demand for online based food/grocery delivery softwares. 

## Problem Statement
In line with those events, this paper aims to use adoption-based probability models to quantify and, in particular, breakdown such changes in order to answer critically important questions that may be asked by the public, the companies and the marketers. 

## Data Source and Description
The main data utilized for this analysis is the daily downloads of the popular online grocery delivery app, Instacart. The data is tracked and supplied by Apptopia, a service that specializes in application tracking. The data at hand consists of Instacart app downloads over 41 days from February 15, 2020 to March 26, 2020. This data is also further supplemented by data gathered from Washington Post on their daily COVID 19 cases updates on the 50 states, the nuance of such addition will be discussed shortly.

## Project Goals
This project overall has three main goals:

### 1.       Accurate Model Creation
This project aims to specify a model architecture that will most effectively capture the underlying drivers pushing Instacart downloads during the COVID-19 crisis. This section will include the underlying stories behind the models, the model assumptions, the parameter choices, and the model evaluation/performance. 

### 2.       Quantitative Impact Assessment
Using the aforementioned model, this project aims to offer immediates and extended inferences as to the extent of changes that COVID-19 has brought upon Instacart downloads. This section will focus on a number of key metrics and answer a number of key questions that need to be addressed.

### 3.       Customer Base Exploration
Capitalizing on the properties of probability models, this paper will also seek to analyze the underlying customer base of instacart including the customer polarity, customer segment and overall customer base size.

## Problem Statement
As indicated, most parts of this project will proceed under the assumption that February 15, 2020 is the first day of instacart’s product launch instead of treating the adoption process as a left censored one. Furthermore, the panel size of this dataset is set to be 120 million, which is roughly equivalent to the number of households in the United States with internet access. 

Furthermore, this is clearly a timing adoption dataset, whereby the time is in fact continuous. However, for the purpose of this analysis and since continuous timing model is really the generalization of discrete timing model, I will still refer to the underlying propensity to adopt using the coin analogy as it is most straightforward. Note that for this case, every coin toss doesn't occur in discrete time units like geometric, but instead it happens at infinitesimally small time slices (practically every mini second, thus virtually continuous in nature). In case of a simple exponential, the lambda estimated is expected to have a direct relationship with the underlying coin, since a higher lambda indicates a faster adoption time and thus a higher propensity.
