# README

## Context 
I've created this python script to use it alone, or in combo with other files, such as Jupyter Notebook. This idea was born while I was trying some code to automatize reading of NaN values in .csv files for a project of Data Manipulation and Visualization. It was so fun, I decided to create another function to extract .zip files and put them in a folder.  

Also, I was thinking about learning git and github, so it seemed a good occasion to get in practice!  

**Note:** If you want to load the script in a Jupyter Notebook without copy and paste, use the magic command `%load book_of_function.py` in an empty cell (this is shown in the notebook file). After running, you will notice that the code in `book_of_function` will import all the code of the script and the magic command will turn into a comment.  

## What's inside this repository? 
Here there are:

- A zip file to test the script;
- The script 'book_of_functions.py';
- A notebook to use in combo with the script if you want.

## The functions

The following functions aim to automatize file extraction and make an overall check about NaN in .csv files:

- `zip_extractor()`, takes as input a folder name. If the folder doesn't exist it's created. Then, it looks for `.zip` files in the same path of this script file path, extracts them, and puts them in the folder provided, or, if not specified, in the same path of this script file;
- `csv_nan_reader()`, This function looks for `.csv` file in a target folder (provided by input), skipping 'checkpoint' files (created automatically by Jupyter), and read them in pandas as DataFrames. Then for each file are printed out: 

	- filename and parental folder;
	- Dataframe shape;
	- number of total cells;
	- number of cells with missing;
	- % of missing data;
	- rows and columns containing missing;
	- rows and columns in original dataset;
	- rows and columns remained after drop;
	- the effect of dropping rows and columns in terms of remaining data and which is the best method.

## Extra, for free, for fun! 
Feel free to download, pull requests, or make suggestions about the script. Hope you can enjoy it or find it as a fount of ispiration!   

## Sources
[Source of the zip file](https://www.kaggle.com/datasets/gsutters/the-human-freedom-index){:target="_blank"}. 