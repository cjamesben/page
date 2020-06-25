---
title: R for Beginners
author: Colin James
date: '2020-06-24'
slug: r-for-beginners
categories: []
tags: []
subtitle: ''
summary: ''
authors: []
lastmod: '2020-06-24T15:28:58-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---



## R Basics

What is R?  How can I use R?  R is an open-source statistical program that can handle anything from basic addition and subtraction to advanced modeling.  It is an amazing resource for anyone in data science, finance, health statistics, etc.  This blog is designed for those who are beginners wanting to learn more about R and its vast array of tools. This blog will become progressively more advanced but it is important to start from a solid base.


### Addition

Updated the variables to calculate eight hundred and fourty seven plus three thousand four hundred and eighty nine.


```r
# Addition
847 + 3489
```

```
## [1] 4336
```

### Subtraction

Update the variables to calculate one thousand three hundred and seven minus eight seven.


```r
# Subtraction
1307 - 87
```

```
## [1] 1220
```

### Multiplication

Let's calculate twelve times ninety


```r
# Multiplication
12 * 90
```

```
## [1] 1080
```

### Division `\(\div\)`

Determine one quarter of five thousand and four.


```r
# Division
5004/4
```

```
## [1] 1251
```





## Session Info


```r
devtools::session_info()
```

```
## ─ Session info ───────────────────────────────────────────────────────────────
##  setting  value                       
##  version  R version 3.5.1 (2018-07-02)
##  os       macOS  10.15.4              
##  system   x86_64, darwin15.6.0        
##  ui       X11                         
##  language (EN)                        
##  collate  en_US.UTF-8                 
##  ctype    en_US.UTF-8                 
##  tz       America/New_York            
##  date     2020-06-25                  
## 
## ─ Packages ───────────────────────────────────────────────────────────────────
##  package     * version date       lib source        
##  assertthat    0.2.0   2017-04-11 [2] CRAN (R 3.5.0)
##  backports     1.1.2   2017-12-13 [2] CRAN (R 3.5.0)
##  blogdown      0.19    2020-05-22 [1] CRAN (R 3.5.1)
##  bookdown      0.19    2020-05-15 [1] CRAN (R 3.5.1)
##  callr         3.4.3   2020-03-28 [1] CRAN (R 3.5.1)
##  cli           2.0.2   2020-02-28 [1] CRAN (R 3.5.2)
##  crayon        1.3.4   2017-09-16 [2] CRAN (R 3.5.0)
##  desc          1.2.0   2018-05-01 [1] CRAN (R 3.5.0)
##  devtools      2.3.0   2020-04-10 [1] CRAN (R 3.5.1)
##  digest        0.6.25  2020-02-23 [1] CRAN (R 3.5.2)
##  ellipsis      0.3.1   2020-05-15 [1] CRAN (R 3.5.1)
##  evaluate      0.14    2019-05-28 [1] CRAN (R 3.5.2)
##  fansi         0.4.1   2020-01-08 [1] CRAN (R 3.5.2)
##  fs            1.4.1   2020-04-04 [1] CRAN (R 3.5.1)
##  glue          1.4.1   2020-05-13 [1] CRAN (R 3.5.1)
##  htmltools     0.5.0   2020-06-16 [1] CRAN (R 3.5.1)
##  knitr         1.29    2020-06-23 [1] CRAN (R 3.5.1)
##  magrittr      1.5     2014-11-22 [2] CRAN (R 3.5.0)
##  memoise       1.1.0   2017-04-21 [1] CRAN (R 3.5.0)
##  pkgbuild      1.0.8   2020-05-07 [1] CRAN (R 3.5.1)
##  pkgload       1.1.0   2020-05-29 [1] CRAN (R 3.5.1)
##  prettyunits   1.1.1   2020-01-24 [1] CRAN (R 3.5.2)
##  processx      3.4.2   2020-02-09 [1] CRAN (R 3.5.2)
##  ps            1.3.3   2020-05-08 [1] CRAN (R 3.5.1)
##  R6            2.2.2   2017-06-17 [2] CRAN (R 3.5.0)
##  remotes       2.1.1   2020-02-15 [1] CRAN (R 3.5.2)
##  rlang         0.4.6   2020-05-02 [1] CRAN (R 3.5.1)
##  rmarkdown     2.3     2020-06-18 [1] CRAN (R 3.5.1)
##  rprojroot     1.3-2   2018-01-03 [2] CRAN (R 3.5.0)
##  sessioninfo   1.1.1   2018-11-05 [1] CRAN (R 3.5.0)
##  stringi       1.2.4   2018-07-20 [2] CRAN (R 3.5.0)
##  stringr       1.4.0   2019-02-10 [1] CRAN (R 3.5.2)
##  testthat      2.3.2   2020-03-02 [1] CRAN (R 3.5.2)
##  usethis       1.6.1   2020-04-29 [1] CRAN (R 3.5.1)
##  withr         2.1.2   2018-03-15 [2] CRAN (R 3.5.0)
##  xfun          0.15    2020-06-21 [1] CRAN (R 3.5.1)
##  yaml          2.2.0   2018-07-25 [2] CRAN (R 3.5.0)
## 
## [1] /Users/colinbenusa/Library/R/3.5/library
## [2] /Library/Frameworks/R.framework/Versions/3.5/Resources/library
```


```r
date()
```

```
## [1] "Thu Jun 25 08:21:32 2020"
```

```r
sessionInfo()
```

```
## R version 3.5.1 (2018-07-02)
## Platform: x86_64-apple-darwin15.6.0 (64-bit)
## Running under: macOS  10.15.4
## 
## Matrix products: default
## BLAS: /Library/Frameworks/R.framework/Versions/3.5/Resources/lib/libRblas.0.dylib
## LAPACK: /Library/Frameworks/R.framework/Versions/3.5/Resources/lib/libRlapack.dylib
## 
## locale:
## [1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## loaded via a namespace (and not attached):
##  [1] knitr_1.29        magrittr_1.5      usethis_1.6.1     devtools_2.3.0   
##  [5] pkgload_1.1.0     R6_2.2.2          rlang_0.4.6       fansi_0.4.1      
##  [9] stringr_1.4.0     tools_3.5.1       pkgbuild_1.0.8    xfun_0.15        
## [13] sessioninfo_1.1.1 cli_2.0.2         withr_2.1.2       remotes_2.1.1    
## [17] htmltools_0.5.0   ellipsis_0.3.1    rprojroot_1.3-2   yaml_2.2.0       
## [21] assertthat_0.2.0  digest_0.6.25     crayon_1.3.4      bookdown_0.19    
## [25] processx_3.4.2    callr_3.4.3       fs_1.4.1          ps_1.3.3         
## [29] testthat_2.3.2    memoise_1.1.0     glue_1.4.1        evaluate_0.14    
## [33] rmarkdown_2.3     blogdown_0.19     stringi_1.2.4     compiler_3.5.1   
## [37] backports_1.1.2   desc_1.2.0        prettyunits_1.1.1
```


```r
date()
```

```
## [1] "Thu Jun 25 08:21:32 2020"
```

```r
Sys.getenv()
```

```
## __CF_USER_TEXT_ENCODING
##                         0x1F5:0x0:0x0
## CENSUS_API_KEY          becc687c781c8c5d1e7dda0c2c046b0c507d217a
## CLICOLOR_FORCE          1
## DISPLAY                 /private/tmp/com.apple.launchd.0WSV3uhIlW/org.macosforge.xquartz:0
## DYLD_FALLBACK_LIBRARY_PATH
##                         /Library/Frameworks/R.framework/Resources/lib:/Library/Java/JavaVirtualMachines/jdk-9.jdk/Contents/Home/lib/server
## EDITOR                  vi
## GIT_ASKPASS             rpostback-askpass
## GITHUB_PAT              bcf752b629b80d38e13a52edb60c5353249a4191]
## HOME                    /Users/colinbenusa
## LANG                    en_US.UTF-8
## LC_CTYPE                en_US.UTF-8
## LN_S                    ln -s
## LOGNAME                 colinbenusa
## MAKE                    make
## MPLENGINE               tkAgg
## PAGER                   /usr/bin/less
## PATH                    /usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin:/Library/TeX/texbin:/opt/X11/bin:/Library/Apple/usr/bin
## PWD                     /Users/colinbenusa/Blog with R
## R_ARCH                  
## R_BROWSER               /usr/bin/open
## R_BZIPCMD               /usr/bin/bzip2
## R_DOC_DIR               /Library/Frameworks/R.framework/Resources/doc
## R_GZIPCMD               /usr/bin/gzip
## R_HOME                  /Library/Frameworks/R.framework/Resources
## R_INCLUDE_DIR           /Library/Frameworks/R.framework/Resources/include
## R_LIBS_SITE             
## R_LIBS_USER             ~/Library/R/3.5/library
## R_PAPERSIZE             a4
## R_PAPERSIZE_USER        a4
## R_PDFVIEWER             /usr/bin/open
## R_PLATFORM              x86_64-apple-darwin15.6.0
## R_PRINTCMD              lpr
## R_QPDF                  /Library/Frameworks/R.framework/Resources/bin/qpdf
## R_RD4PDF                times,inconsolata,hyper
## R_SESSION_TMPDIR        /var/folders/m8/4ph0yk_12zddg0z7btxz7tp80000gn/T//Rtmp1znpod
## R_SHARE_DIR             /Library/Frameworks/R.framework/Resources/share
## R_SYSTEM_ABI            osx,gcc,gxx,gfortran,?
## R_TEXI2DVICMD           /usr/local/bin/texi2dvi
## R_UNZIPCMD              /usr/bin/unzip
## R_ZIPCMD                /usr/bin/zip
## RMARKDOWN_MATHJAX_PATH
##                         /Applications/RStudio.app/Contents/Resources/resources/mathjax-26
## RS_PPM_FD_READ          25
## RS_PPM_FD_WRITE         54
## RS_RPOSTBACK_PATH       /Applications/RStudio.app/Contents/MacOS/rpostback
## RS_SHARED_SECRET        2824752491622650073984943658
## RSTUDIO                 1
## RSTUDIO_CONSOLE_COLOR   256
## RSTUDIO_CONSOLE_WIDTH   107
## RSTUDIO_PANDOC          /Applications/RStudio.app/Contents/MacOS/pandoc
## RSTUDIO_SESSION_PORT    34856
## RSTUDIO_USER_IDENTITY   colinbenusa
## RSTUDIO_WINUTILS        bin/winutils
## SED                     /usr/bin/sed
## SHELL                   /bin/bash
## SHLVL                   1
## SSH_ASKPASS             rpostback-askpass
## SSH_AUTH_SOCK           /private/tmp/com.apple.launchd.oNyQnin255/Listeners
## TAR                     /usr/bin/tar
## TERM                    xterm-256color
## TMPDIR                  /var/folders/m8/4ph0yk_12zddg0z7btxz7tp80000gn/T/
## USER                    colinbenusa
## XPC_FLAGS               0x0
## XPC_SERVICE_NAME        org.rstudio.RStudio.1432
```




