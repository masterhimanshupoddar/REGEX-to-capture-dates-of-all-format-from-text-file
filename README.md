# REGEX-to-extract-dates-of-all-format-from-text-file
This repo extract dates from text file of any format


Here is a list of some of the variants : <br>
04/20/2009; 04/20/09; 4/20/09; 4/3/09 <br>
Mar-20-2009; Mar 20, 2009; March 20, 2009; Mar. 20, 2009; Mar 20 2009 <br>
20 Mar 2009; 20 March 2009; 20 Mar. 2009; 20 March, 2009 <br>
Mar 20th, 2009; Mar 21st, 2009; Mar 22nd, 2009 <br>
Feb 2009; Sep 2009; Oct 2010 <br>
6/2008; 12/2009 <br>
2009; 2010 <br>

The example text file can found in the repo

Supppose you want to matcha character but does not want to capture it, you can use ?=character

To save in a xlsx file <br>
from pandas import ExcelWriter <br>
writer = ExcelWriter(r'C:\Users\Himanshu Poddar\Desktop\Coursera courses\Applied text mining with python\assignment1dates.xlsx') <br>
fg.to_excel(writer,'Sheet1') <br>
writer.save() <br>
