Abstract
=================================

**Increasing access to the NHANES 1988-2018 surveys & mortality linkage data via a user-friendly Stata program**

Wilson Gomez, MHS
Johns Hopkins Bloomberg School of Public Health

**Background:** 
Stata is one of the go-to statistical software used for statistical analyses; however, Stata lacks the ability to push interactive content to the internet. Additionally, Stata users are limited due to file incompatibilities and computational power. These limitation make it difficult to analyze big survey data like NHANES. To address Stata's limitations, we designed a program to access and display the NHANES US mortality data from 1959-2017 in a virtually accessible book.

**Methods:** 
We used the Stata `dyndoc` command to turn the Stata do file into a html file. Additionally, we used Python to build a jupyter book and push the Stata content to GitHub. Below is an example of the pertinent code used to create the book. 

````
dyndoc nhanes-stmd.do, saving(nhanes.html)
````

To push the content to the virtual book we used the following hack: 

````
jupyter-book build mybook 
cp -r mybook/* myrepo 
cd myrepo
git add ./*
git commit -m "My first hack"
git push 
ghp-import -n -p -f _build/html
````

To see the code used to create the US Mortality Trends graph, see [dyndoc](https://wgomez1.github.io/myrepo/Chapter2.html).

**Results:** 
The program imported the NHANES US mortality data and displayed the trend in the graph below. 
<<dd_do:nooutput>>
qui do https://raw.githubusercontent.com/jhustata/book/main/nhanes-alpha.ado      
set scheme s2color
nhanes

<</dd_do>>


<<dd_graph>>


<<dd_do>>

use nh3andmort, clear
di "obs: `c(N)' & vars: `c(k)'"  
<</dd_do>>


**Conclusions:** 
If we want to promote open science, we need softwares such as Stata to incorporate features allowing users to publish content publicly online. This project demonstrates  a way to overcome Stata's limitation. 

**References:**

1. https://jhustata.github.io/book/jjj.html
2. https://jupyterbook.org/en/stable/start/your-first-book.html
3. https://www.stata.com/stata-news/news36-1/spotlight-markdown/
4. https://wwwn.cdc.gov/nchs/data/nhanes3/1a/adult.sas
5. https://jhustata.github.io/class700/intro.html
6. https://www.jhsph.edu/courses/course/37447/2022/340.700.71/advanced-stata-programming
7. [Muzaale AD. Databases for surgical health services research: National Health and Nutrition Examination Survey. Surgery. 2019 May;165(5):873-875](https://www.surgjournal.com/article/S0039-6060(18)30076-X/fulltext)
8. https://www.ssc.wisc.edu/~hemken/Stataworkshops/dyndoc%20review/Review.html
