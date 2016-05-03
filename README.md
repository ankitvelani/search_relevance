Product Search Relevance
========================

This is the code to solves the HomeDepot's data science challenge on Kaggle
 [[+]](https://www.kaggle.com/c/home-depot-product-search-relevance).
 Our solution gives the RMSE score of 0.458 and scored at 72 out of 2125 (*top 3.5%*)
 spot in the leadboard. 

Overview of the ML pipeline:
---------------------------

![alt tag](https://github.com/rmanak/search_relevance/blob/master/img/ML_homedepot.png)



Preparation:
-----------

In ``project_params.py`` edit the following to the correct path

     - ``input_root_dir``: the path to the original .csv files in your system
     - ``output_root_dir``: a path with few GB disk space avaiable for I/O

Requirements:
-------------

0) To do all of the following (1,2,3) you can simply use:

    ``make install``

1) To install the required packages execute:

    ``pip install -r requirements.txt``

The project needs the following python packages:
   -numpy
   -pandas
   -scikit-learn
   -nltk

2) You may also need to install nltk data:

  - in python:

    ``>>> nltk.download()``

  - or via command line:

    ``python -m nltk.downloader all``

  - or makefile will take take care of everythin:

    ``make install``

(Particularly nltk_utils uses WordNet data.)


Initial Test:
-------------

run ``make testutils`` to check if things work!




Run:
----

See the content of ``run_all`` for the flow of runs

