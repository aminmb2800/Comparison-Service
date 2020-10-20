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

As a computer student, I am eager to learn a lot in this field.
This code can show equal values in the final file but can not show inequality in one line.
I hope I can find a solution to this problem with your help.

[Back To The Top](#Comparison-Service)

---

## Technical problems

I used .merge() functionality in pandas to compare the differences between the two data frames.  
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

My name is Mohammad Amin Mohammadi Banadaki. I have been working in various fields such as mathematics that  
I working on testing of micro technology , C++ and working at fraunhofer on web scraping with python using libraries ('beautifulsoup','request','selenium') and collect data with SQLite.  
I have been working scientifically in the field of Python for two years and I have decided to learn more and more in this field, especially data science.I can quickly learn and use the material, so I learned Python in depth and I am still very interested in learning it, which eventually led to teaching this subject at university and It would be great 
if I learn from those who work experimentally and effectively in this field, like your team.As a team player, I am collaborative with peers, searching for ways to integrate valuable insights. 


[Linkedin](https://www.linkedin.com/in/aminbanadaki/) 
