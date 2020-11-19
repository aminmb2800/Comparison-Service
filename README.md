# Comparison-Service

Comparing the Extraction invoice based on Ground Truth invoice and present it as CSV summary file.

### Table of Contents

- [Description](#description)
- [Feedback Of Result](#feedback-of-result)
- [Technical Problems](#technical-problems)
- [Installation](#installation)
- [Usage](#usage)
- [Author Info](#author-info)

---

## Description

To better understand some of content, you should use the principle of testing, which leads to a better understanding of the work process.  
In this case, the company wants to check the accuracy of its extraction model for the services it provides.  
By having a 'Ground truth' that contains basic and fixed information that determines the amount and type of services.  
Extracted items called 'Extraction' which are a random example of services provided by the company that with Ground truth are compared and finally the proximity of their output is checked.
By quantifying the equality and inequality of the data, it can be compared as a whole. A value of '0' for equality of columns and a value of '1 'for inequality checks .


[Back To The Top](#Comparison-Service)

---

## Feedback Of Result

This code can show equal values in the final file and can show inequality in one line.

[Back To The Top](#Comparison-Service)

---

## Technical problems

I used .merge() functionality in pandas to compare the differences between two data frames.  
I had trouble establishing all the conditions for this output, which eventually led to separate values in different rows. 

[Back To The Top](#Comparison-Service)

---

## Installation

Install [pandas] (https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html)  
To install pandas with conda run:

```bash
conda install -c anaconda pandas
```
[Back To The Top](#Comparison-Service)

---

## Usage

usage of [.merge()](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.merge.html)

Sample: 

```python
import pandas as pd 

df1 = pd.DataFrame({'lkey': ['foo', 'bar', 'baz', 'foo'], #dataframe1
                    'value': [1, 2, 3, 5]})
df2 = pd.DataFrame({'rkey': ['foo', 'bar', 'baz', 'foo'], # dataframe2
                    'value': [5, 6, 7, 8]})
                    
df1.merge(df2, left_on='lkey', right_on='rkey')  #merge both and shows the differences 

```

[Back To The Top](#Comparison-Service)

---

## Author Info

[Linkedin](https://www.linkedin.com/in/aminbanadaki/) 
