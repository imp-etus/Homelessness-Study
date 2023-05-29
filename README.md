# US Homelessness Modeling: Market Factors and Homeless Rates
## Overview
This repository holds a DATA 3320 project exploring how to model the relationship between market factors and homelessness. Using Housing & Urban Development data, we aim to explore the relation between market factors & homelessness, as well as models of community-level homelessness & see if we can outperform HUD models on the topic.

## Data
The raw data for the file is taken from the 2019 Market Predictors of Homelessness HUD report and is in this repository as `05b_analysis_file_update.csv`. A dictionary explaining the column is stored here as `HUD TO3 - 05b Analysis File - Dictionary.csv`. The HUD report explaining the data can be found [here](https://www.huduser.gov/portal/sites/default/files/pdf/Market-Predictors-of-Homelessness.pdf). 

### Data Processing

In order to prepare the data, we used a Colab notebook, referred to here as Data Preparation.ipynb. We renamed most columns to readable names, as well as removing all years with incomplete data sets. This left us with 2017 data. Furthermore, we had to convert all homelessness data to homelessness per 10,000 people, because otherwise dense urban areas would have disproportionate homelessness predictors & we wouldn't be able to compare different districts 

## Requirements

We used a Colab/Jupyter notebook to perform all analysis. However, this could just as easily be done with a standard Python client & the libraries linked in each notebook. 

## Conclusion

We were unable to predict the data with much certainty. Our root mean-squared error using ridge regression was 21.41, and our lasso regression results were too spread out to be of any value in predictions. We found a loose correlation between city districts & increased rates of homelessness, but each mean was within a standard deviation of each other, and there's not really much we can glean from that. 

## Authors

Evelyn McCarty

Notable help from Long Tran-Thien, which is why certain sections of our work look similar. 

## License

MIT License

Copyright (c) 2023 evelyn mccarty

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
