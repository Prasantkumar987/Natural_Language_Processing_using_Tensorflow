# IMDB movies rating (using Tensorflow)

Here I built a model to rate a movie on the basis of dataset of IMDB rating.<br>
I used the dataset for this from Tensorflow, there this dataset is in-built in datsets call of tensorflow and you can use it by clicking [Here](https://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz).<br>
You can take help of IMDb.ipynb file where I coded it,available in this folder.<br>

This model is already trained on Tensorflow's website. Accuracy of the model on the website is 0.8351 with validation accuracy 0.7864.<br>

I achived the accuracy of 0.88 with 0.83 validation accuracy but it was overfitting so I used Dropout with Adamax optimizer and added additional Hidden layer again I achieved accuracy of **0.8835** with **0.8308** validation accuracy.<br>


### Parameters:
Number of neurons = 32<br>
Number of hidden layers = 2<br>
Droputout = 0.5 and 0.2<br>
activation function = relu<br>
optimizer = Adamax<br>
loss = binary_crossentropy<br>
metrics = accuracy<br>
epochs = 20  <br>


### Plotted the accuracy on Tensorboard
Its awesome to plot accuracy and loss on Tensorboard simply using the logs which get created during model training.
                                                  ![image](https://user-images.githubusercontent.com/54981696/118462001-d9bd6480-b71b-11eb-947b-387de9246a28.png)


### You should also try it out. 

