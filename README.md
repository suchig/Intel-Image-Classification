# Intel-Image-Classification

**Objective**
To recommend an architecture to classify ~15K images into 6 classes.

**Data**
Kaggle Intel images - https://www.kaggle.com/puneet6060/intel-image-classification

**Description**
Image_Classification_Intel_images.ipynb
- Visualized clusters by creating t-SNE of images
- Created custom models of architecture using different combinations of Convolution, Pooling, Batch Normalization, Dropout and Fully Connected layers
- Augmented the images and classified them using a complex architecture of two sets of Conv/Pool/Dropout and a final Fully connected layer. This improved the accuracy and reduced the loss
- Created Transfer Learning based models using Inception V3, MobileNet and VGG. Used a learning rate of 0.00001 for the optimzer.
- Recommended VGG owing to an accuracy of nearly 90% and a steady decrease in loss between training and validation sets

Embedding_Visualization_using_Tensorboard.ipynb
- Created a sprite of all test images
- Created an embedding features set by removing the last layer of the model and predicting for the test images.
- Created checkpoint data, meta data(Not to be confused with label meta data) and index file using Tensorboard plugins.
- Created configuration file using Visualize Embeddings
- Outside of the notebook, the following has to be done to visualize t-SNE
  - Run Tensorboard --logdir=LOG_DIR_PATH
  - Go to localhost:6006 to visualize the tensorboard

