# Tikur Chest X-ray Imaging Dataset

[![KB license](https://img.shields.io/badge/license-AAU-brightgreen.svg)](#)

## Disease Categories

```bash
Atelectasis, Cardiomegaly, Effusion, Infiltration, Mass, Nodule, Pneumonia,
Pneumothorax, Consolidation, Edema, Emphysema, Fibrosis, 
Pleural_Thickening and Hernia
```

## Overview

Suppose you have an image dataset in a directory which looks like this:

```
FileName	Atelectasis	Cardiomegaly	Effusion	Infiltration	Mass	Nodule	Pneumonia	Pneumothorax	Consolidation	Edema	Emphysema	Fibrosis	Pleural_Th	Hernia
jat011.jpg	      0 	    0    	    0     	     0 	        0	    1	     0   	      0	             0	          0 	     0      	  0 	             0	          0
kal012.jpg	      0 	    0    	    0     	     0 	        0	    0	     0   	      0	             0	          0 	     0      	  0 	             0	          0
kem013.jpg	      0 	    0    	    0     	     0 	        0	    0	     0   	      0	             0	          0 	     0      	  0 	             0	          0
mat014.jpg	      0 	    0    	    0     	     0 	        1	    0	     0   	      0	             0	          0 	     0      	  0 	             0	          0
mes015.jpg	      0 	    0    	    1     	     0 	        0	    0	     0   	      0	             1	          0 	     0      	  0 	             0	          0
seb016.jpg	      0 	    0    	    0     	     0 	        0	    0	     0   	      0	             1	          0 	     0      	  0 	             0	          0
she017.jpg	      0 	    0    	    0     	     0 	        0	    0	     0   	      0	             0	          0 	     0      	  0 	             0	          0
.
.
.
kas028.jpg	      0 	    0    	    0     	     0 	        0	    0	     1   	      0	             0	          0 	     0      	  0 	             0	          0
kid029.jpg	      0 	    0    	    0     	     0 	        0	    0	     0   	      1	             0	          0 	     0      	  0 	             0	          0
mek030.jpg	      0 	    0    	    0     	     0 	        1	    0	     0   	      0	             0	          0 	     0      	  0 	             0	          0
mul031.jpg	      0 	    0    	    0     	     0 	        0	    0	     1   	      0	             0	          0 	     0      	  0 	             0	          0
mus032.jpg	      0 	    0    	    0     	     0 	        0	    1	     0   	      0	             0	          0 	     0      	  0 	             0	          0
.
.
.
elf198.jpg	      0 	    0    	    0     	     0 	        1	    1	     0   	      0	             0	          0 	     0      	  0 	             0	          0
get199.jpg	      0 	    1    	    1     	     0 	        0	    0	     0   	      0	             0	          1 	     0      	  0 	             0	          0
kas200.jpg	      0 	    0    	    0     	     0 	        0	    0	     0   	      1	             0	          0 	     0      	  0 	             0	          0

```

You can use this image dataset for training:

```
Programming Language
Python 

 ```

All images in the dataset must have the same shape , it was originally extraced with an image resolution of 664 x 680.
Also, you can validate your models using this real-world dataset

