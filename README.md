# Machine Learnig and Its Mathematical Basis
by Torey Hilbert (November 2017)

Goal
--------------------
I studied the math behind Decision Trees, K-Means, and Artificial Neural Networks. Instead of using libraries, I used Python code in a Jupyter Notebook to recreate these algorithms from scratch.


Clustering Algorithm: K-Means
--------------------
I selected a K-Means algorithm and the Iris dataset.

The key parameters for clustering are a distance measure and the number of clusters (the k). I sampled a few distance metrics, but settled for the Manhattan distance. I found 9 clusters gave the highest accuracy. 

Data: In the Iris dataset each row represents a unique iris flower, including its sepal length, sepal width, pedal width, and species. The target is to accurately predict/group by plant species. My code loads this dataset from the sklearn library (iris dataset), but the same data is also available from UCI ML: http://archive.ics.uci.edu/ml/datasets/Iris


Artificial Neural Networks Algorithm: Backpropagation
--------------------
I selected a feed-forward with backpropagation algorithm and the MNIST image processing dataset.

I used 4 layers in my network, with 784 neurons in the first, 30 neurons in the second and third, and 10 in the output layer. During training, I split the data into batches of 25 rows and ran each batch three times, updating in between. I also varied a training step parameter which describes how much the weights are changed during each trial. I measured error using sum of squares.

Data: MNIST is dataset of human handwritten numbers with labels. The full MNIST dataset has 60,000 training examples and 10,000 testing examples. A subset is available in the sklearn library (the digits dataset). I used the full dataset which is available at: https://www.kaggle.com/zxstest/handwritten-digits/code  