README COVID19 Project 							      4/26/2020
by Francisco Lacruz and Raul Lorenzo
****************************************************************************************

On this document I will explain how to use the different .ipynb documents of the project

***********************************COVID19_SORT_DATA************************************

This notebook is used to sort the original data folder into a new data folder separated 
into train, test and validation.

DATA_PATH = Directory for the downloaded data folder "New Data". 
If you want to try the function sort_data, you can just delete the images from the other 
data folder ("Sorted Data") and then execute the program.

**********************************COVID19_TRAIN_TEST_1**********************************

This is the notebook used to train the models and evaluate the models.

DATA_PATH = Directory of the "Sorted Data" folder.
MODEL_PATH = Directory of the folder where you want to save the models after training.

**********************************COVID19_TRAIN_TEST_2**********************************

This was an extra notebook with the same function as COVID19_TRAIN_TEST_1. It trains the
last architecture. We had to create this extra notebook due to the lack of GPU Memory. 


**************************************COVID19_CAM***************************************

This is the notebook used to create the Class Activation Map.

DATA_PATH = Directory of the "Sorted Data" folder.
MODEL_PATH = Directory of "model_Xception_CAM_epochs_20_optimizer_adam_batch_32.h5".

This model architecture was not directly implemented from the keras library in order to 
access into the Xception Convolutional layers.

The training of that new model can be seen on this notebook but you can just upload the 
given model "model_Xception_CAM_epochs_20_optimizer_adam_batch_32.h5".

The last block of this notebook plots the CAMs of three random images from the training
set.

************************************COVID19_TEST_MODEL**********************************

This notebook is for evaluate the models without training.

DATA_PATH = Directory of the "Sorted Data" folder.
MODEL_PATH = Directory of the models given.