# PCA-algorithm-from-scrath

The main idea of PCA (Principal component analysis ) is to find patterns and reduce the dimension of the dataset with a minimal loss of information .
So , here we have loaded the mnist dataset . Have build the pca algorithm from scratch with the respective steps :

1 . First thing we have to do is to normalize the dataset . Even when you are using the sklearn.decomposition.pca . We normalized using statistical Z value
            
                  Z = datapoint - (mean of whole datapoint) / standard deviation
             
2 . We convert dataframe to numpy array for faster computation .

3 . Take the mean of every row to adjust to the origin .

4 . finding x.xT as we need to max the sum of 1/m(x.T*u)^2 after simplyfying to sum of u*x.xT*u.T .

5 . Find the covariance matrix .

6 . Find the eigen value and eigen vector of covariance matrix .

7 . From eigen value take the first 2 highest eigen value to plot a 2-D .

8 . Having 2 eigen vectors of 2 highest eigen is called Transformation matrix .

9 . move the points to origin mnist-mnist_mean .

10 . projection of data points to our eigenvector .

11 . We finally check with the sklearn.decomposition.pca how similar they are .
