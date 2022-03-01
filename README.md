
# Face Mask Detection

The Model is designed to check if any human is wearing a mask or not.

  
## Dataset Description

The Dataset contains a total of 11,792 images divided in three folders  

* Test (992 images),  
* Train (10,000 images),   
* Valid (800 images),  

Each of these folders has sub-folders :

* **Test**  
  * WithMask   
  * WithoutMask 
  
* **Train**  
  * WithMask   
  * WithoutMask  

* **Valid**  
  * WithMask   
  * WithoutMask    

you can download the dataset [here](https://www.kaggle.com/vasanthgowdamk/face-mask/download)


## Convolution Base (VGG19)

![image](https://user-images.githubusercontent.com/97322648/156185628-7fbaf454-74ae-44f9-aa6b-856504316a1d.png)


to import the model, run 

```bash
  from tensorflow.keras.applications import VGG19
```

## Result


![__results___17_0](https://user-images.githubusercontent.com/97322648/156185725-4c1ae3a3-5f1d-4444-948c-5549bb5d9a5f.png)


The training stablized due to early stopping after achieving the following parametrs 

| Accuracy | in percentage |
| ------------- | ------------- |
| Training Accuracy| 99.62  |
| Validation Accuracy | 99.75  |
| Testing Accuracy |1.0|

| Loss | in decimal  |
| ------------- | ------------- |
| Training loss| 0.0213  |
| Validation loss |  0.0760  |
|Testing loss |5.9828e-04|

The model trained for 16 epochs before early stopping conditions were met. 
