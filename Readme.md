In the last decade, the world has seen a series of fatal respiratory illnesses transmitted from person to person through droplets 
when someone with the virus coughs, sneezes, talks, shouts, or sings. The current respiratory illness in the world is COVID-19,
With 31,731,754 confirmed COVID cases and 570,436 deaths in U.S and this number increasing rapidly not only in USA but around the world, 
it is everyone’s responsibility to protect themselves and others from this virus. 

Even though CDC and government have rapidly increased the vaccination administration, a mask mandate is compulsory.
Masks can act as simple barrier to help prevent your respiratory droplets from reaching others.
Our project would be helpful in situations where people do not obey the rules in public places and help containing the disease. 
Have used a Convolutional Neural Network (CNN) model to help detect people who wear a mask and those who do not wear it.

Exploratory Data Analysis
The dataset consists of 2 folders, “with mask” and “without mask”. 
Have a total of 7553 images and out of those 3725 images are “with mask” and 3828 images are “without mask". 

Initially have loaded the required libraries which would help in the image path detection and while modelling. 
After setting up the path to the image data folders, converted the images into grayscale and then resized each image into 112 x 112 size to maintain consistency
and for better model building. Then used one hot encoding to categorize the images into the classes “With mask” and “Without mask”. 
Then split 75% data into training set and 25% into validation/test set.

Model
Using the keras package, built a basic sequential model with 2 layers containing the
features Conv2D, ”Relu” Activation function, Max-Pooling, Flatten, Dropout and a dense layer with “softmax” activation. Further, set the number of epochs to 50. 

Next, built a sequential model with 3 layers containing the features Conv2D, ”Relu” Activation function, Max-Pooling, Flatten, Dropout 
and a dense layer with “softmax” activation. The epochs used are 50

The best validation accuracy able to achieve after several parameter tuning is 92.44%.

Conclusion
While the accuracy of our best model is 92.44% it can still act as a good enforcement mechanism for the mask mandate. 
Unlike a situation where the accuracy is highly critical, like the COVID-19 test, can still use this model in a real-life situation with the above accuracy. 
The trade-off in gaining higher accuracy could be slower processing. The slower processing could be negated through higher computing resources and more data. 
But then we might be limiting the implementation to only those business entities with high revenue. 
