# Importing Data Using Pandas - Lab

## Introduction

In this lab, you'll get some practice with loading files with summary or metadata, and if you find that easy, the optional "level up" content covers loading data from a corrupted csv file.

## Objectives
You will be able to:

- Use pandas to import data from a CSV and and an Excel spreadsheet  

##  Loading Files with Summary or Meta Data

Load either of the files `'Zipcode_Demos.csv'` or `'Zipcode_Demos.xlsx'`. What's going on with this dataset? Clean it up into a useable format and describe the nuances of how the data is currently formatted.

All data files are stored in a folder titled `'Data'`.


```python
# Import pandas using the standard alias

```


```python
# Import the file and print the first 5 rows
df = None

```


```python
# Print the last 5 rows of df

```


```python
# What is going on with this data set? Anything unusual?
```


```python
# Clean up the dataset

```

## Level Up (Optional) - Loading Corrupt CSV files

Occasionally, you encounter some really ill-formatted data. One example of this can be data that has strings containing commas in a csv file. Under the standard protocol, when this occurs, one is supposed to use quotes to differentiate between the commas denoting fields and the commas within those fields themselves. For example, we could have a table like this:  

`ReviewerID,Rating,N_reviews,Review,VenueID
123456,4,137,This restaurant was pretty good, we had a great time.,98765`

Which should be saved like this if it were a csv (to avoid confusion with the commas in the Review text):
`"ReviewerID","Rating","N_reviews","Review","VenueID"
"123456","4","137","This restaurant was pretty good, we had a great time.","98765"`

Attempt to import the corrupt file, or at least a small preview of it. It is appropriately titled `'Yelp_Reviews_Corrupt.csv'`. Investigate some of the intricacies of skipping rows to then pass over this error and comment on what you think is going on.


```python
# Hint: Here's a useful programming pattern to use
try:
    # Do something
except Exception as e:
    # Handle your exception e
```

## Summary

Congratulations, you now practiced your Pandas-importing skills.
