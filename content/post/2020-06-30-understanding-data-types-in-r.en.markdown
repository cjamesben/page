---
title: Understanding Data Types in R
author: Colin James
date: '2020-06-30'
slug: understanding-data-types-in-r
categories: []
tags: []
subtitle: ''
summary: ''
authors: []
lastmod: '2020-06-30T20:40:05-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

## Data Types

A data type is an attribute of data that gives a programmer an indicator of how the data will be used. In R there are a wide assortment of data types that include scalars(character, numeric, logical, integer, complex), vectors, matrices, and data frames.  It is important to know the data type of each variable in a dataset before analyses can be done.  Data types can make calculations faster and more efficient depending on the analyses.


### Scalars

Scalars are data types that hold only one type at a time, whether it be a character, numeric, logical, integer, or complex. We are going to download a multitude of datasets through the 'datasets' package in R to look at some examples of data types. 

Character variable data types are usually alphabetic but always require "" when used in a dataset. Ex: "Apple", "Porsche", "Tom"... etc.

Numeric is self exaplanatory.  This datatype is the most common data type that I encounter and include anything, well numeric.  Ex: 9494, 950300, 00008... etc.  The two most common types of numeric data types are integer and double.

1)Integer is a numeric data type that stores whole numbers, anything from negative to positive values.  For SQL servers,integers range from -2,147,483,647 to 2,147,483,647.  
  
2)Double is a numeric data type that stores numbers with up to 17 decimals.  Ex.  59903.99595959

Logical is a special data type with only two possible values.  Ex: 0/1, true/false, yes/no, etc.  I typically use logical data types as a flag variable if I want to identify if a condition exists or not.


Complex data type is anything that is not included in the previous data types.  Example is 1 - 2i, see example below


```r
# numeric is probably the most common data type you will encounter in data science

# downloading 'datasets' package
library(datasets)

# viewing all datasets in the package
data()

# picking 'mtcars' dataset to view. Head function gives us a quick glance at all of the columns
head(mtcars)
```

```
##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1
```

```r
# 'str' function like the head function lets us view all variables in the dataset but lists the data types in the dataset as well
str(mtcars)
```

```
## 'data.frame':	32 obs. of  11 variables:
##  $ mpg : num  21 21 22.8 21.4 18.7 18.1 14.3 24.4 22.8 19.2 ...
##  $ cyl : num  6 6 4 6 8 6 8 4 4 6 ...
##  $ disp: num  160 160 108 258 360 ...
##  $ hp  : num  110 110 93 110 175 105 245 62 95 123 ...
##  $ drat: num  3.9 3.9 3.85 3.08 3.15 2.76 3.21 3.69 3.92 3.92 ...
##  $ wt  : num  2.62 2.88 2.32 3.21 3.44 ...
##  $ qsec: num  16.5 17 18.6 19.4 17 ...
##  $ vs  : num  0 0 1 1 0 1 0 1 1 1 ...
##  $ am  : num  1 1 1 0 0 0 0 0 0 0 ...
##  $ gear: num  4 4 4 3 3 3 3 4 4 4 ...
##  $ carb: num  4 4 1 1 2 1 4 2 2 4 ...
```

```r
#Here we can see the UC Berkley Admissions dataset that contains character variables
str(UCBAdmissions)
```

```
##  'table' num [1:2, 1:2, 1:6] 512 313 89 19 353 207 17 8 120 205 ...
##  - attr(*, "dimnames")=List of 3
##   ..$ Admit : chr [1:2] "Admitted" "Rejected"
##   ..$ Gender: chr [1:2] "Male" "Female"
##   ..$ Dept  : chr [1:6] "A" "B" "C" "D" ...
```

```r
#Example of complex data type.  The 'class' function is used to determine the data type.
z = 1 + 2i

z
```

```
## [1] 1+2i
```

```r
class(z)
```

```
## [1] "complex"
```


### Vectors

A vector is a basic data structure that always contain elements of the same type


```r
# the '<-' is used to store values in a variable, and 'c()' is the combine function
 x <- c(9, 4, 5, 6, 7, 10)

#all values in this data structure are double
typeof(x)
```

```
## [1] "double"
```

```r
#Because vectors contain elements of the same type, this function will try to convert all values in the vector to one data type.  This conversion occurs from lower to higher types, from logical to integer to double to character, with character data type being the most influential
x <- c(1, 5.4, TRUE, "hello")

x
```

```
## [1] "1"     "5.4"   "TRUE"  "hello"
```

```r
# Here we can see that all values were converted to a character data type
class(x)
```

```
## [1] "character"
```

```r
#There are many caveats to vectors but for the sake of staying on topic, we will discuss in another post
```



### Matrices

Matrices are data structures that are two dimensional, and like vectors will contain values of all the same data type.

Personally I do not use matrices all that much, except maybe correlation tables related to stock analyses, but otherwise they are important to know about.


```r
#You can create a matrix using the 'matrix' function matrix(data, nrow, ncol, byrow, dimnames)
M <- matrix(c(1:45), nrow=5, byrow = TRUE)

#new function 'print' shows the input value or matrix
print(M)
```

```
##      [,1] [,2] [,3] [,4] [,5] [,6] [,7] [,8] [,9]
## [1,]    1    2    3    4    5    6    7    8    9
## [2,]   10   11   12   13   14   15   16   17   18
## [3,]   19   20   21   22   23   24   25   26   27
## [4,]   28   29   30   31   32   33   34   35   36
## [5,]   37   38   39   40   41   42   43   44   45
```

### Data Frames

Data Frames are the data type that most people are familiar with. Like matrices, data frames are two dimensional structures but contain variables that can be composed of different data types such as numeric, character or logical.  Data frames have rows and columns, usually with rows of unique observations


```r
data()

#Looking at Freeny's Revenue Data.  
head(freeny)
```

```
##               y lag.quarterly.revenue price.index income.level market.potential
## 1962.25 8.79236               8.79636     4.70997      5.82110          12.9699
## 1962.5  8.79137               8.79236     4.70217      5.82558          12.9733
## 1962.75 8.81486               8.79137     4.68944      5.83112          12.9774
## 1963    8.81301               8.81486     4.68558      5.84046          12.9806
## 1963.25 8.90751               8.81301     4.64019      5.85036          12.9831
## 1963.5  8.93673               8.90751     4.62553      5.86464          12.9854
```

```r
class(freeny)
```

```
## [1] "data.frame"
```


Hope this information has been helpful.
