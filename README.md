# REGEX to extract dates of all format from a text file
The code extracts dates present in any format from  a text file.

A Sample test file is present at `dates.txt`

### Date variants the code can extract : 

| 1. | 04/20/2009 | 04/20/09 | 4/20/09 | 4/3/09 |
|---|------------|----------|---------|--------|

| 2. | Mar-20-2009 | Mar 20, 2009 | Mar. 20, 2009 | Mar 20 2009 |
|---|------------ |----------|---------|--------|

| 3. | 20 Mar 2009 |20 March 2009 | 20 Mar. 2009 | 20 March, 2009  |
|---|------------ |----------|---------|--------|

| 4. | Mar 20th, 2009 |Mar 21st, 2009| Mar 22nd, 2009 |
|---|------------ |----------|---------|

| 5.| Feb 2009 | Sep 2009 | Oct 2010 |
|---|------------ |----------|---------|

| 6.| 6/2008 | 12/2009 | 
|---|------------ |----------|

| 7.| 2009 | 2010 | 
|---|------------ |----------|

#### Supppose you want to match a character but do not want to capture it,use `?=character`

### To save in a xlsx file
```
from pandas import ExcelWriter 
writer = ExcelWriter(r'C:\Users\Himanshu Poddar\Desktop\Coursera courses\Applied text mining with python\assignment1dates.xlsx') 
fg.to_excel(writer,'Sheet1')
writer.save()
```
