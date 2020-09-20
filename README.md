# ml-raw-logistic-regression

***Introduction***  
This notebook presents step by step implementation of a binary classifier for MNIST dataset, where we distinguish following classes(digits 0 and 1 are supposed to be removed from the dataset):
- Prime nubmers(2,3,5,7)
- Compound numbers(4,6,8,9)

The solution is going to:
 - Implement both **logistic regression** and optimization ***SGD + momentum*** using only **numpy**.
 - Tune the hyperparameters in order to increase the performance on test set.
 - Evaluate the model.

***Requirements:***
- python-mnist (Data reader)
- matplotlib
- seaborn
- numpy
- sklearn (for validation purposes only)

***Download MNIST***

(train set):
 - http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz
 - http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz
 
(test set):
 - http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz
 - http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz

***Unpack the data and rename the files***

 replace "." to "-" for all of the files names:  
   - **train-images.idx3-ubyte**   ->  **train-images-idx3-ubyte**  
   - **train-labels.idx1-ubyte**   ->  **train-labels-idx1-ubyte**  
   - **10k-images.idx3-ubyte.gz**   ->  **10k-images-idx3-ubyte.gz**  
   - **10k-labels.idx1-ubyte.gz**   ->  **10k-labels-idx1-ubyte.gz**  

