# Tikur Anbessa Specialized Hospital :  image dataset 

[![AAU license](https://img.shields.io/badge/license-AAU-brightgreen.svg)](#)

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

The shape of the `x_*` arrays will be `(instances, rows, cols, channels)` for color images and `(instances, rows, cols)` for grayscale images.
Also, the shape of the `y_*` arrays will be `(instances,)`.

All images in the dataset must have the same shape.
Also, all data subsets (i.e., `train` and `test` in this example) must contain the same set of classes.
Class names will be sorted alphabetically.
So, in this example, `cats` and `dogs` will be represented by `0` and `1`, respectively.

You can also load a single data subset. For example:

```python
(x_train, y_train), = image_dataset_loader.load('./data', ['train'])
```

Note that the comma after `(x_train, y_train)` is required, because the function always returns a tuple of tuples.

## API

```python
load(dataset_path, set_names,
     shuffle=True, seed=None,
     x_dtype='uint8', y_dtype='uint32')
```

- **`dataset_path:`** Path to the dataset directory.
- **`set_names:`** List of the data subsets (subdirectories of the dataset directory).
- **`shuffle:`** Whether to shuffle the samples. If false, instances will be sorted by class name and then by file name.
- **`seed:`** Random seed used for shuffling (see the [docs](https://docs.python.org/3/library/random.html#random.seed)).
- **`x_dtype:`** NumPy data type for the X arrays (see the [docs](https://numpy.org/devdocs/user/basics.types.html)).
- **`y_dtype:`** NumPy data type for the Y arrays (see the [docs](https://numpy.org/devdocs/user/basics.types.html)).
- Returns a tuple of `(x, y)` tuples corresponding to `set_names`.
