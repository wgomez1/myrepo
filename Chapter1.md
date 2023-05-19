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
[Graph](https://wgomez1.github.io/myrepo/nh3andmort.svg)

**Conclusions:** 
If we want to promote open science, we need softwares such as Stata to incorporate features allowing users to publish content publicly online. This project demonstrates  a way to overcome Stata's limitation. 
