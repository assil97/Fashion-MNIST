# Fashion-MNIST

Fashion MNIST is a dataset provided by the keras containing the photos of T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle Boot in the format of gray where the size of the photos is 28 * 28 * 1.

Few examples of the Fashion MNIST Images are: 

![Fashion MNIST](mnist.png)

Fashion MNIST contains 60000 training images and 10000 testing images along with the targets that are uniquely assigned to the images making a total of 70000 images and targets.

Images are normalized by dividing every image by 255 which will return the value between 0 and 1.

Fashion MNIST was trained in Convolutional Neural Network in four layers where two layers are CNN Layers and the remaining two layers are Dense Layers where the activation layers are Relu and Softmax for nomalization.

The CNN architecture is as follows:-

   1. CNN Layer 1
      
      Layer 1 contains around 14 batches where padding is valid by default and the kernel size is 3 * 3 
      which is followed by MaxPoolingLayer where the size is 2 * 2 and the input_shape of the image is 28 * 28 * 1.
      
   2. CNN Layer 2
      
      Layer 2 contains around 28 batches where padding is valid by default and the kernel size is 3 * 3 
      which is followed by MaxPoolingLayer where the size of the matrix is 2 * 2.
     
   3. CNN Layer 3
      
      Layer 3 is known as Flatten Layer where the tensor shape is reshaped to equal number of elements i.e 
      reshaping image  shape of three dimensions to the number of images.

   4. CNN Layer4 
      
      Layer 4 is known as Dense Layer where it consists of deeply connected neural network with a total of 128 units and           relu activation layer for normalization of array where each value is between 0 and 1.

   5. CNN Layer 5
      
      Layer 5 is the last layer followed by Dropout Function which is used to avoid overfitting in the model by selecting a       few units of neural network bearing more probability than others bearing the value of 0.3. The last layer in CNN             contains only 10 units for classifying 10 fashion objects to predict the image that can be determined by returning the       highest value of the probability among the objects with softmax activation function.
       
The metrics used in this classification is accuracy to calculate how well the CNN Model have predicted the image among the 10 fashion objects and the accuracy of the model is 89.41%.
