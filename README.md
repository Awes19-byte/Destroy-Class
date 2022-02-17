# Ensemble of Pre-trained models for Image Classification
![This is an image](https://miro.medium.com/max/605/1*wp3kI8A53ygpeflOnRqMfw.png)
## **Prerequisite** 
``` Python 3.X ``` <br/>
``` Tensorflow 2.X ``` <br/>
``` Numpy ``` <br/>
``` Pandas ``` <br/>
## **Pre_trained Models**
- Xception : [Documentation](https://keras.io/api/applications/xception)
- MobilnetV2 : [Documentation](https://keras.io/api/applications/mobilenet)
- InceptionV3 : [Documentation](https://keras.io/api/applications/inceptionv3)
## **Steps**
**1. Load data and Fine tune the pre-trained models** <br/>
**2. Create your customized data genertor** <br/>
you need to build your own data generator to feed the pre-trained models simultaniously 
in this exemple i used three pre-trained models so i create a data generator that generate 
3 copies of data for training and one label. So it's depend on the number of pre-trained models to use <br/>
**3. Build the combinaison** <br/>
First of all we need to define our input and output of our model then we will use the functional API 
Concatenate the models and the dense layers
