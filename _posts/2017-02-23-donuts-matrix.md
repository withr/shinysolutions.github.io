---
layout: post
title:  "Donuts matrix"
date:   2017-02-23 17:40:06
categories: highcharts
image: donuts-matrix.png

---


Donuts matrix using Highcharts. There are two parts of **highcharts.js** need to be modified:

- line 224: change function "C" to "parseFloat". This will allow accurate position for *center* option of highcharts. 

- line 207: insert "this.userOptions.w||" before "this.containerWidth", and "this.userOptions.h" before "p(a,this.containerHeight>19". This will make sure the size of output figure changes as row/column number changed.
 

[Source code](https://github.com/shinysolutions/donuts)

<iframe src="http://51.175.77.204/donuts/"></iframe><br>

