# **Exploration of "PyScript"**

&nbsp;   
This will be my documentation of the usage of PyScript and how it works.  


&nbsp;  
&nbsp;  
&nbsp;  

## **Installation**
---
&nbsp;  
The installation is really easy since it is just a matter of doing the script link with  
```html:
<link rel="stylesheet" href="https://pyscript.net/alpha/pyscript.css"/>  
<script defer src="https://pyscript.net/alpha/pyscript.js"></script>
```
&nbsp;  

## **Writing in python**
---
&nbsp;  

When it comes to actually writing code you will be writing within an html element in the following fashion  

```html:
</py-script>
    <!-- python code goes here -->
</py-script>
```
or using a src:
```html:
<py-script src="./test.py">  </py-script>
```
&nbsp;  
There is a pretty shitty code highlighter available in the VS extensions called "HardeepSingh.pyscript" if you want some level of code highlightning
&nbsp;  
&nbsp;  

## **Python third party installs (pip)**
---

The third party installs are handled in a pretty nice way as you just include:
```html:
<py-env>
    - matplotlib
</py-env>
```
Only a select few modules seems to be working with PyScript at the moment. Plotly for example did not work at all.  
&nbsp;


## **General python syntax**
---

* Prints will just print straight into the html and it will mirror a console. So doing a for loop and printing will result in a long line and not an updated element.
* You can't comment using `//` but instead have to do a html comment `<!-- --> ` within the PyScript tag
* 
&nbsp;