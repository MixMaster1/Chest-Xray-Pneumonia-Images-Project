# Machine Learning and Pneumonia
![X-Ray Image](./chest_xray/test/NORMAL/IM-0001-0001.jpeg)
In this project I will attempt to make a nueral network that can predict wether a patient has Pneumonia or not using x-ray images. The goal is to help doctors by freeing up their time doing other important stuff instead of wasting time on looking at X-rays.

# Data Set
My Data set came from <a href='https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia'>
    *Kaggle*
</a>. The file contains about a total of 5,863 X-Ray images in Jpeg format and categorized under Pneumonia and Normal.
There are 3 other folders one with train images, test images, and validation images all of which add up to the total amount of 5,863. One thing I changed in the data folder was drag more images from the train folder into the validation folder since I could not get the full scope of my models with the very little images in the validation folder.

# Work Flow
I started off by reshaping my images and having my train images set my train_y and my test and t_val.
I ran 8 different models the very first 3 modules I had only one layer to test out what each method will do like over fit my model or underfit it. The fourth model was a combination of methods to increase our metric accuracy. I found my Models were not completely finished learning from my training images to the next model I ran with more epochs. I then tried convolutional nueral networks. I tried many different methods with My CNN models and they all roughly stayed the same accuracy. Towards my last model I realized accuracy is not the right metric to use in this type of problem. We want to make sure our models can predict more true negatives than true positives. We dont want to send a patient home thats actually sick.

My recall scores for my final 2 models were 0 which I found odd and that means my models were all predicting 
that the patients are healthy which in this case we want to avoid.

# Conclusion
Nueral networks can be used in this type of problem medically I would just have to improve the models to a point where we can relaibly diagnos a patient thats sick using this model.

# Next Steps
I want to improve my models recall score to above a .5 and move on up from there.
Once I have a good recall score I would like to see my model predict both categories succesfully that way we can have doctors focus their man power somewhere else.