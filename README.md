# Description

This project aims to build a recommender system for movies [Movielens data](https://grouplens.org/datasets/movielens/100k/) based on [Factorization Machines Method](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)

The data transformation was made using [numpy](http://www.numpy.org/) [pandas](https://pandas.pydata.org/), and the Matrix factorization implementation was done with [Tensorflow api](https://www.tensorflow.org/)

As input, we have the feature vector matrix as you can see in the picture bellow :


![Alt text](images/facto_input.png?raw=true "Title")


As output, we obtain the latent representation of each feature (see the paper)

Finally, in order to compute the rating for the pair (i, j), we use the factorization machine formula : 

![Alt text](images/facto_machine_formula.PNG?raw=true "Title")

We evaluate the performance of the algorithm using RMSE metric as in the paper.

You will find the Implementation + Data Transormation + Algorithm Evaluation in the [notebook](https://gitlab.eurecom.fr/amadeus/Factorization_Machines/blob/master/Factorization_Machine.ipynb)