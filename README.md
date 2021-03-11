Blood Cell Subtypes Classification

Dataset- Blood Cell Images
This dataset contains 12,500 augmented images of blood cells with accompanying cell type labels . There are approximately 3,000 images for each of 4 different cell types grouped into 4 different folders (according to cell type). 
The cell types are Eosinophil, Lymphocyte, Monocyte, and Neutrophil. This dataset is accompanied by an additional dataset containing the original 410 images as well as two additional subtype labels and also bounding boxes for each cell in each of these 410 images.
 The folder 'dataset2-master' contains 2,500 augmented images as well as 4 additional subtype labels.

![Blood Cell Classes](https://user-images.githubusercontent.com/66276711/110815102-25810700-82b0-11eb-9d74-a6cb6eee2279.png)

 
Model Summary

![S1](https://user-images.githubusercontent.com/66276711/110815537-89a3cb00-82b0-11eb-9d78-b1882588e9a4.png)
![S2](https://user-images.githubusercontent.com/66276711/110815688-ab04b700-82b0-11eb-9b7d-b42d19efc694.png)


The above Convolutional Neural Network classifies the 4 classes of blood cells- Eosinophils, Monocytes, Lymphocytes and Basophiles after training.
This model has 6 convolution layers, 2 dense layers, 7 dropouts and approximately 220K parameters.
It gives 80% and 79% accuracy for 20 epochs.

Accuracy Incremention
Following methods were using in the above model to increase accuracy:
Increased the number of convolution layers from 2 to 6 which caused a  significant increase in accuracy.
Decreased the number of neurons in the convolution layers and connecting layers which led to a huge increase in accuracy %
The model started overfitting so we added Dropouts to the convolution layers and decreased the Dropout values from 0.7 and 0.5 to values of 0.4 and 0.3 in the connecting layer. 


Accuracy	 
![Accuracy](https://user-images.githubusercontent.com/66276711/110814995-ff5b6700-82af-11eb-848f-67cb4f069583.png)


Loss		 
![Loss](https://user-images.githubusercontent.com/66276711/110814802-ccb16e80-82af-11eb-9e9f-2e9cdf71ea2f.png)



