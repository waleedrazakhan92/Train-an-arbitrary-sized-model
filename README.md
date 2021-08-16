# Train-an-arbitrary-sized-model
This repository aims to tackle the problem of input size restriction on pretrained models. Whenever we train the model or use a pretrained one, you can only perform inference on the same size the model was trained on. This severely restricts the use of the model. 
A VGG16 architecture is chosen to train, where there is no restriction to model input image size. 
For experimentation the Intel Image Classification dataset is downloaded, via code, in the notebook. But if you find the link broken, you can download the same dataset from https://www.kaggle.com/puneet6060/intel-image-classification . For faster training, please make sure that the runtime is set to "GPU".

Please see the .ipynb file for model training code.

Instructions
Place the dataset and set the path to variable "path_dataset".
Set the batch size to a value that easily fits in the gpu memory.
Set the image size to a desired value. Make sure that it is in the power of 2, i.e (64,128,256,512).
Start the training.
**Note** All the code is tested in google colab with both tensorflow 1.14 and 2.0.
