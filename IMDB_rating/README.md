# IMDB movies rating (using Tensorflow)

Here I built a model to rate a movie on the basis of dataset of IMDB rating.<br>
I used the dataset for this from tensorflow, there this dataset is in-built in datsets call of tensorflow and you can use it by clicking [Here](https://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz).<br>
You can take help of IMDb.ipynb file where I coded it,available in this folder.<br>

## Steps
### Importing Dataset
I imported the dataset of Imdb rating from url given above. And using that url, I downloaded the dataset into file which got saved into the directory. After that I imported the dataset form my directory using function **text_dataset_from_directory** from preprocessing class <br>

### Data Preprocessing
There are few steps which I have followed to make data reliable which can be used to train model:<br>
1.Adding **Embedding layers**<br>
2.Added a **Custom Standardization** function which converts words in Lowercase, removes HTML tages and Punctuations also<br>
3.**Tokenisation** of words after implementing Custom Standardization<br>

### Building CNN Model
There are few steps which I have followed to build IMDb model which are following:<br>
1.**Vectorised** the inputs using vectorization layer function
2.Added **Embedding layers** containing 1000 vocabolary words and 5 dimensions<br>
3.Added **GlobalAveragePooling1D** layer
4.Added **Dense layers**<br>
5.**Dropout Layer**<br>
6.Again added **Dense Layers** for full connections.

### Training Model
1.Compile the model on optimizer, loss, and metrics<br>
Before fiting our training data into model, we have to compile our model from best paramters for data to get best results out of it.<br>
  I used **Adamax** optimizer because it worked best for this dataset.<br>
  I used **Binary_crossentropy** for loss because here we have only classes, so this loss function is best to deal with it.<br>
  I used **accuracy** for metrics parameter.<br>
2.Fiting data and training model on dataset<br>
  Here I fitted my data on model and used by testing data for validating the model and callbacks.<br>
  I tried 35 epoches to train this model and got accuracy on validation data of **0.8292** .It took me about 02 mins to train it.<br>
  
### Plotted the accuracy on Tensorboard
Its awesome to plot accuracy and loss on Tensorboard simply using the logs which get created during model training.
                                                        ![image](https://drive.google.com/file/d/12wNesc9nRPAQMvv4emZQhQkNzMB3xt4x/view?usp=sharing)   

### You should also try it out. 

