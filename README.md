# DLFinalProjectGroup-5
**Group Members**
Martin, Maximino III
Ommi, Naga Amani
Palepu, Balachander-301170247
Patel, Vishal-301169302
**Supervised learning**
Imported kaggle API credentials to collab
Used keras,numpy,mathplotlib,pandas libraries
Loaded dataset from kaggle into dataframe
Seggregated dataframe intlo lables(labels) and features(df_labels)
-Labels : There are 400 bird species
Created ImageDataGenerator to randomly rotate images and rescaled to 1/255(img_loader)
Loaded data from train,test,valid folders into images_train,images_test,images_valid respectively.
-Found 58388 images belonging to 400 classes from train.
-Found 2000 images belonging to 400 classes from test.
-Found 2000 images belonging to 400 classes from validation.
Model Construction using CNN model
-Configured CNN to process inputs of (180,180,3)
-We build a sequential model and added convolutional layers and max pooling layers to it.
-For training the model, the batch normalisation technique was used, which standardises the inputs to a layer for each mini-batch.
-We also added dropout layers in between,used relu activation.
-We added dense layers at the end which are used for class prediction(0–9) with softmax as activation
-Summary of the model is 
  -Total params: 2,235,184
  -Trainable params: 2,234,544
  -Non-trainable params: 640
-Model fit with training and validation data with epochs=25 and batch_size=256
 -accuracy:0.7780
 -loss:1.0318
-Evaluated model for testing data
 -accuracy:0.8025
 -loss:0.8578
