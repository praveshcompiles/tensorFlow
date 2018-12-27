## Image classification using TensorFlow

Image_classification_using_TensorFlow.ipynb

This notebook demonstrates the image classification of Belgian traffic signs. 

### Background: 
There are six categories of traffic signs in Belgium: warning signs, priority signs, prohibitory signs, mandatory signs, signs related to parking and standing still on the road and, lastly, designatory signs.
On January 1st, 2017, more than 30,000 traffic signs were removed from Belgian roads. These were all prohibitory signs relating to speed.
The overwhelming presence of traffic signs has been an ongoing discussion in Belgium (and by extension, the entire European Union).


#### The problem:  62 types of traffic signs needs to be classified correctly.


62 labels for 62 types of traffic signs

Images are converted to matrix values

Images are transformed to grayscale (classification vs detection)

Rescale the images to 28x28  (784-dimensional)

Define placeholders for inputs and labels because ( “real” data is not yet put)

Flattening of the input - making it linear

A fully connected layer that generates logits , is constructed
Logits is the function operates on the unscaled output of earlier layers

Multi-layer perceptron 

Loss function: softmax cross entropy  - measures probability in discrete classification tasks 

Optimizer - Stochastic Gradient Descent (SGD) 

When the session is finally ran, the placeholders get the values of the dataset that is passed in the run() function
