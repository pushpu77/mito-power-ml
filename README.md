# mito-power-ml

# Image segmentation 
It was performed by implementing the U-Net architecture with both basic trainable weights and pretrained weights from ResNet, EfficientNet, and MobileNet. 

# DataSets
Two types of datasets were used to implement the segmentation model:

Real Images Dataset: This dataset comprises 60 corresponding face and eye masks. It was primarily used in transfer learning. <br>
SBVPI Dataset: This dataset was used for training the basic U-Net model, providing a significant amount of data for robust model training.
Augmentations were applied to both datasets to remove location invariance and enhance model performance.

# Comparison
The different models were compared based on their validation and training loss and accuracy. This comparison helped in identifying the best-performing model among those trained with basic weights and those utilizing pretrained weights from ResNet, EfficientNet, and MobileNet.

# Classification

For jaundice classifier the images were segmented from the best model (EfficientNet) in this case and saved into the main directory. All the datasets used in the image segmentation and classification is present in the private google drive link https://drive.google.com/drive/folders/1h8fCdlmqsghjhL-Wrc2z48lTex8Glb1e?usp=sharing. 

# Codes

The code for end-to-end-image classifier is present under the folder end-to-end-segmentation-jaundice-classifer. The code is written in the ipynb format. The model that has been used is pretrained ResNet50 model from keras. The metrics (loss and accuracy) graph are also been attached within the code for your reference. 

# Inferences

We can see the improvement in accuracy in classification to more than 95%. Segmenting the eyes for the classification removes all the biases and unnessary training. Therefore we can see such good results with small datasets. Although we can improve the model by training the segmentation model with more data. 
