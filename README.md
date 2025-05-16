# Computer-Vision
Authors: Christian Gonzalez, Anthony Manese, Raul Gallardo Trejo

How to run the code:
Our models was created, tested, and ran in Jupyter Notebooks. Ensure the data path is correct when running on your own machine. Run all cells in Jupyter and it should execute 
and give the same performance as we got.

Brief explanation of key files and functions:

New label file for test images: **test.csv** This is a key file because it was not provided before.
**train.csv** holds the labels for the training images
**test** and **train** folders hold the images we used to train and test our models
**label_num_to_phase_map.json** explains what each label corresponds to

For CNN
Although our CNN model file doesn't rely heavily on functions, a key block of code is Block 11, where we build the model and fine-tune it. This block shows the steps we took, 
from the architecture we used like dense layers, dropout layers, to the hyper-parameters that allowed us to get the performance we did.

For BOVW
Some key functions within our Bag of Visual Words files include:

build_vocabulary: This function shows the process we used to create the vocabulary from images.

Block 54: This block demonstrates how we stitched back together the pipeline after separating images that couldn’t be classified due to not having any key features. It shows a 
more complex pipeline than that of the CNN, which does it all end to end.

These features are especially important because they show creativity and ingenuity. We had to not only figure out new techniques, but also how to break up a problem — like when 
SIFT couldn’t distinguish black and flat images — and create a method that picked up that dead weight but still worked toward the same goal.
