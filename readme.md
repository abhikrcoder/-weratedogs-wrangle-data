# @weratedogs Wrangle Report 
## by Abhishek kumar


## Dataset

> Wrangling the data is 80% of total work so they say, this is report of a Data
wrangling project of twitter site @weratedogs which rates dogs. This project is
consists of three parts gathering the data by downloading by url and also by
API.Assessing the data by visualising and programmatically and then Cleaning
the data by extracting the meaningful data.


## Gathering

> Gathering Data for this Project involved obtaining three different datasets from
three different sources. Each one testing a different way of obtaining a dataset.
The first was to download a file manually and be able to open a csv file. In this
case the file was called “twitter_archive_enhanced.csv” and was the file
consisting of the largest amount of data. Which I have given by the Udacity
yourse itself so no work needed for that.
The second was to be able to download a file programmatically using Python
Requests library. The file contained image predictions on the breed of the dog
coming from a neural network on some of the tweets already downloaded in the
archive file. The file was in tsv format and tested your ability to open this type of
file successfully.
The final dataset is slightly complicated and tested ability we uses Twitter’s API
and use a Python library called Tweepy to obtain further data on the tweets in the
archive file using the tweet id. First we required to use twitter api credentials and
then the Tweepy library returned the data in json format, from which it was
possible to iterate through and append data to a file as a list of dictionaries and
then a pandas data frame. A copy was saved in csv format of the data frame
created. 

## Assessing

> The three saved data frames were then assessed visually inside a jupyter notebook
with pandas and because the datasets were not too large, a copy of each was
exported into one Excel workbook. This allowed quick scanning through the rows
and use of filters to identify areas for more detailed investigation. Following this
a programmatic assessment was made inside jupyter with pandas using the
following functions, df.info(), df.head(), df.sample(10) (several different samples
were taken), df.value_counts().
The datasets were accessed under two criteria, quality and tidiness. When an
issue was detected it was documented under one of these two criteria.
Quality refers to issues related to the content of the data, sometimes called dirty
data. The standard criteria of completeness, validity, accuracy, and consistency of
the data were used to identify quality issues. Tidiness refers to issues related to
the structure of the data, sometimes called messy data. The basis for assessment is
that each variable forms a column, each observation forms a row and each type of
observational unit forms a table. After assessing the three datasets, it was decided
to marge them into a single data frame, reducing superfluous columns that
wouldn’t be needed in any future analysis. 

## Cleaning
>The final step in the wrangling process is cleaning the data for quality and
tidiness issues. We have accessed the data and now based on that we need to
clean our data. For missing value we just drop the columns and change the wrong
datatype. And lastly we merge the cleaned data set.

## Conclusion
>Data wrangling provides a clean data frame for future analysis and visualization,
in our case we concluded with the “twitter_archive_master.csv’.
