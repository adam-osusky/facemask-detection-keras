# Facemask detection

The Covid-19 pandemic is a global health crisis that has affected the world. It is one of the greatest challenges, that humanity is facing today. One of the effective methods of protection is wearing a facemask in public areas. The aim of this work is to create a system that will perform facemask detection and could be used for further development to a particular implementation. This work provides jupyter notebook demonstrating procedure for creating such a system. The main elements of the solution are an artificial neural network(ANN) and the haar-cascade classifier program(OpenCV). Haar-cascade classifier is detecting the positions of faces and ANN is deciding wheter the face is with or without a mask. In this work the transfer learning method is used and MobileNetV2, with weights trained on ImageNet, is the basis of the ANN. In this repository you can find model which was trained on 3000 images from Kaggle[1]. The accuracy of the model on test data was 97.1%.(test data consisted of 1000 images) The resulting system can execute facemask detection. Alas, the model is far from perfect, there is a lot to improve. The model can make accurate classifications only in favorable situations, i.e., the person is looking into the camera and the camera is not moving. This system can serve as a proof of concept for future development of more accurate and better facemask detection systems. It can also be a good starting point in some specific implementation of facemask detection system.  


[1] Kaggle datasets  
https://www.kaggle.com/prasoonkottarathil/face-mask-lite-dataset/version/1  
https://www.kaggle.com/vinaykudari/facemask/version/2  
https://www.kaggle.com/sumansid/facemask-dataset/version/2
## Getting Started

In this repository you can find: jupyter notebook for creating and fitting the model(model_training), jupyter notebook for testing the model on camera on your machine(testing_webcam), model fitted on 3000 images-saved with Keras(trained_model).

## Built With

* [TensorFlow](https://www.tensorflow.org/api_docs) - deep learning library (Keras)
* [Matplotlib](https://matplotlib.org/3.3.3/contents.html) - library for graphs
* [OpenCv](https://docs.opencv.org/master/) - auxiliary library for computer vision
