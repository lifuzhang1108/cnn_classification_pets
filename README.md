# cnn_classification_pets
### requirement tensorflow 2.0.0
### check this post on host to install
https://stackoverflow.com/questions/55392100/install-tensorflow-2-0-in-conda-enviroment

### the main function is at the end of the python notebook
```
X,y = read_data()
Xtrain, ytrain, Xtest, ytest=split_data(X,y,20)
yguess,yguess_train=cnn(Xtrain,ytrain,Xtest)
print("training accuracy",calculate_accuracy(ytrain, yguess_train))
print("test accuracy",calculate_accuracy(ytest, yguess))
```
### to apply new test datasets, simply reinitialize  Xtest and ytest
### the function cnn() builds the convolutional neural network using the training data
### it takes about 2 minutes to run and generate arount 97% test accuracy
