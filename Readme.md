# Snoring sound classification using deep learning
## Project: This project uses a simple deep learning model to classify the snoring sounds from the non snoring ones

### Install

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://jupyter.org/install.html) or any other IDE to run notebooks on your local machines

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](https://www.anaconda.com/download/) distribution of Python, which already has the above packages and more included. 

### Code

THe code is provided in the `snoring-classification.ipynb` notebook file. You will also be required to download and included the `snoring dataset` dataset file from `Kaggle` to run the file. Meanwhile if your machine doesnoth have a GPU it is advicable to use the google colabs.


### Run

In a terminal or command window, navigate to the top-level project directory `snoring-classification/` (that contains this README) and run one of the following commands:

```bash
ipython notebook boston_housing.ipynb
```  
or
```bash
jupyter notebook boston_housing.ipynb
```
or open with Juoyter Lab
```bash
jupyter lab
```

This will open the Jupyter Notebook software and project file in your browser.

### Data
The dataset contains two folders - one for snoring and the other for non-snoring.

Folder 1 contains snoring sounds. It has total 500 sounds. Each sound is 1 second in duration.
Among the 500 snoring samples, 363 samples consist of snoring sounds of children, adult men and adult women without any background sound. The remaining 137 samples consist of snoring sounds having a background of non-snoring sounds.

Folder 0 contains non-snoring sounds. It has total 500 sounds. Each sound is 1 second in duration.
The 500 non-snoring samples consist of background sounds that might be available near the snorer. Ten categories of non-snoring sounds are collected, and each category has 50 samples. The ten categories are baby crying, the clock ticking, the door opened and closed, total silence and the minor sound of the vibration motor of the gadget, toilet flashing, siren of emergency vehicle, rain and thunderstorm, streetcar sounds, people talking, and background television news.


### Model
1.  Model has 5 layers
2.  Out of the the we have used 2 convolution layers and 2 dense layers.
3.  We have used the sigmoid layer as the activation layer for the final layer since this is a binary classification problem.
4.  Model was train based on the Adam optimizer.



### Results
After training the model for 10 epochs
1.  Accuracy - 1.0000
2.  loss -  0.0025
3.  val_recall - 1.0000

