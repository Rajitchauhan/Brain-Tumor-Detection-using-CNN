# Brain-Tumor-Detection-using-CNN
# Abstract :
 A brain tumor is regarded as one of the most competitive diseases among children and adults. The majority of number one Central Nervous System (CNS) malignancies are brain tumors, which account for 85 to 90% of all CNS tumors. Every year, around 11,700 people are diagnosed with a brain tumor. Humans with a malignant mind or CNS tumor have a 5-year survival rate of around 34 percent for men and 36 percent for women. There are three types of brain tumors: start tumor, middle tumor, and end tumor. Malignant Tumor, for example, requires proper treatment, planning, and diagnostics in order to improve the patients' life expectancy. Magnetic Resonance Imaging (MRI) is a great way to detect brain cancers (MRI). 
 
# Introduction :
According to the National Brain Tumor Society, around 700,000 people in the United States have a brain tumor, with the figure rising to 787,000 by 2020 [1]. A brain tumor is not usually more common than other malignancies such as breast cancer or lung cancer, but it is nevertheless the 10th leading cause of death worldwide. Brain cancer is expected to kill 18,020 persons in the next 12 months [2]. A brain tumor has a long-term and mental impact on the lives of those who are affected. A brain tumor develops as a result of tissue damage. An anomaly that develops in the brain or within the main backbone and disrupts normal brain function. There are two types of brain tumors: benign and malignant. Benign brain tumors are benign tumors that do not contain cancer cells and grow slowly. They do not spread and usually live in a single part of the mind, but malignant mental tumors contain cancer cells and develop quickly, spreading to other areas of the mind and backbone. A malignant tumor is both dangerous and life-threatening. The World Health Organization (WHO) has classified brain tumors into grade 1 and 2 low-grade tumors (also known as benign tumors) and grade 3 and 4 high-grade tumors (also known as malignant tumors) based on brain health behavior 

# Objective : 
#### Our main objective is to detect a brain tumor from MRI (Magnetic Resonance Image) using CNN (Convolutional Neural Network) .
###
#### We developed a model which is able to detect a brain tumor from MRI using CNN , we used a brain MRI data founded on kaggle.
#### - The Name of Datasets is 'Dataset Br35H'.
'Dataset Br35H' :   https://www.kaggle.com/ahmedhamada0/brain-tumor-detection
#### - The Datasets contain two folder , one is 'yes' and another is 'no'.
#### - The folder 'yes' contain MRI that is tumous and 'no' contain non-tumous.
#### - We also  used another folder named 'pred' folder , which is used for prediction our model.

# Related Work
Hossain et al. proposed an approach to detect[6].They proposed using the Fuzzy C-Means clustering algorithm, followed by standard classifiers and convolutional neural networks, to extract brain tumors from 2D magnetic resonance brain images (MRI). The experiment was conducted on a real-time dataset with tumors of various sizes, locations, forms, and.Intensities

Suhib Irsheidat, et al. proposed an approach to detect[7]They proposed a model based on Artificial Convolutional Neural Networks that uses mathematical formulas and matrices operations to evaluate magnetic resonance pictures. This neural network predicts the likelihood of a tumor in the brain, and it was trained using magnetic resonance images with 155 healthy brains and 98 tumors. There are 253 magnetic resonance pictures in total in the dataset.

Pankaj Sapraet al. proposed an approach to detect[8],Modified image segmentation algorithms were used on MRI scan images to detect brain tumors in this study. A modified Probabilistic Neural Network (PNN) model based on learning vector quantization (LVQ) with image and data analysis and manipulation techniques is also proposed in this paper for performing automatic brain tumor classification using MRI-scans. The training performance, classification accuracies, and computing time are all used to evaluate the updated PNN classifier's performance.


# Proposed Work
In this research, we implemented Image Processing and Data Augmentation strategies on a small dataset of 808 brain MRI images. We trained them through a easy Convolution layers CNN model and as compared our scratched CNN model . The dataset consists of 667 images of malignant cancer and 343 of benign non-cancerous tumors. We break up our dataset into 3 separate segments for training, validation, and testing. The training information is for model learning, validation information is pattern information for version assessment and model parameters tuning. Test information is for the final evaluation of our model. Our proposed technique consists of diverse phases


## A. Image processing
First, we cropped the dark edges from the images and took simplest the brain component from MRI images with the aid of using the usage of Open source Computer Vision (CV) Canny Edge Detection technique[9]. Canny Edge Detection is a multi-segment algorithm used to perceive the edges of an object in an image. In Fig 3, The edges of the Real MRI brain have shown the usage of the canny edge detection technique after which simplest the brains part of the image has been cropped

![image](https://user-images.githubusercontent.com/45984646/175514889-f1e30b08-f89d-4594-ac87-adfbf46ec916.png)

## B. Data augmentation
Data Augmentation is a method for artificially growing the amount and complexity of present facts. We recognize that training a deep neural community desires a big quantity of facts to fine-tune the parameters [9]. But our dataset may be very small, so we carried out the method of facts augmentation on our education dataset with the aid of using including changes to our photos with the aid of using making minor adjustments, which include flipping, rotation, and brightness. It will growth our training data length and our model will keep in mind every of those small adjustments as a wonderful image, and it's going to allow our version to research higher and carry out well on unseen data. 

![image](https://user-images.githubusercontent.com/45984646/175515041-e0943fd7-c7de-43bd-b104-1c984c0109d9.png)

## C. CNN Model (Convolutional Neural Network)
CNN is a deep learning model for processing data with a grid pattern, such as images, that is inspired by the structure of animal visual cortex [13] and designed to learn spatial hierarchies of characteristics from low- to high-level patterns automatically and adaptively. Convolution, pooling, and fully connected layers are the three types of layers (or building blocks) that make up a CNN. The first two layers, convolution and pooling, extract features, while the third, a fully connected layer, transfers the retrieved features to final outputs like classification. Convolution, a specific sort of linear operation, is a major component of CNN, which is made up of a stack of mathematical operations. Pixel values are stored in a two-dimensional (2D) grid, i.e., an array of numbers and a small grid of parameters called kernel, an optimizable feature extractor, is applied at each image position, making CNNs[11] highly efficient for image processing because a feature can appear anywhere in the image. Extracted features can become hierarchically and progressively more complicated as one layer feeds its output to the next layer.

![image](https://user-images.githubusercontent.com/45984646/175516525-d1852026-1e1e-4c16-bf8f-f5d27e599f3e.png)


## Work Flow of Proposed method

1. Load input data
2. Resizing the images
3. Max Pooling feature
4. Adding Convolution layer
5. Flattering
6.	Processing of the vector in dense layer
7.	Final dense layer applying Sigmoid as the Activation Function






## Model and Training
#### The model consists of:

* CNN Layer
* Max Pooling Layer
* Dense Layer
* Fully Connected Layer
* Loss Function: Categorical Cross-Entropy
* Optimization Algorithm: Adam

#  Result : 
Testing is one parameter that might determine whether your work is successful or not. Testing the CNN is a key stage in the process of CNNs. Since the tests, evaluate the CNN and ensure that it is accurate How accurate are your predictions in identifying the proper result? label. Testing can also reveal issues with the CNN, such as an example of over fitting We used 80% of the data for training and 20% for analysis. for testing purposes We spent two weeks putting our CNN through its paces. different songs for it in order to find the perfect one structure and excellent precision We put the CNN to the test. different loss functions and different optimizer algorithms We experimented with different filter numbers and tried to optimize the layers. Sizes of filter.

![Acc99](https://user-images.githubusercontent.com/45984646/175520183-ca64bc62-6a82-40dc-b292-e3c959261755.JPG)


Model is trained on 25 epochs.

Model | Accuracy | Loss
| :--- | ---: | :---:
CNN Proposed method  | 99.81% | 0.0192%

### Model Accuracy :

![image](https://user-images.githubusercontent.com/45984646/175507341-24c55b8a-2a1f-4f0d-9889-3ca944bab920.png)

### Model Loss

![image](https://user-images.githubusercontent.com/45984646/175507184-38bb552c-aed2-4917-a57c-214bd5c58dfd.png)


### Compare our model with existing model . 

Methodology  | Accuracy(%)
------------- | -------------
Hossain et al.[6]  | 97.87
Suhib Irsheidat et al.[7]  | 96.7
Hassan Ali Khan et al. [9]  | 98.51
Proposed CNN Model   | 99.81

# Future Scope
Improve computational time by using boosting techniques using data augmentation  , fine-tuning hyper parameter i.e. using adding more appropriate layers.
Classifier boosting is done by building model from the training data then creating a second model that attempt to correct the error from first model for faster prognosis. Such technique can be used to raise the accuracy even higher and reach a level that will allow to be asset to any medical facility dealing with brain tumor. 


# Conclusion 
A new strategy to classifying brain tumors was presented in this research. We first found the region of interest in MRI pictures and cropped them using the image edge detection approach. Increasing the size of our training data using data augmentation. Second, we offer a cost-effective solution .A basic CNN network is proposed as an approach for brain tumor classification. For elegant and sophisticated precise outcomes The training of a neural network demands a vast quantity of data, but our results were promising.We created an CNN to identify MRI scans as positive (labeled as 1) or negative (labeled as 0), indicating whether or not the individual has a tumor. We tested our CNN with a test data set and observed that it has an evaluation accuracy of 90.25%. We finally developed an Artificial Convolution Neural Network that can predict brain tumors from MRI brain images, with forecasting accuracy of up to 88.25 % on test data and 99.81 % on assessment data. We plan to further refine the CNN, tune it with the best tunes and settings, and train it with more data, either from other sources or by adding more augmentation to existing images.



# References
[1].NBTS, National Brain Tumor Society: Quick brain tumor facts, 2020. Available from:
https://braintumor.org/brain-tumor-information/brain-tumor-facts/.
[2]. Cancer. Net, Brain Tumor: Statistics, 2020. Available from:https://www.cancer.net/cancertypes/brain-tumor/statistics.

[3]. NHS, National Health Service: Brain Tumors, 2020. Available from:
https://www.nhs.uk/conditions/brain-tumours/.

[4]. Normal Brain image  Available from: 
https://prod-images-static.radiopaedia.org/images/17420180/78de707f66bbf12bf2da188b96bb2e_big_gallery.jpeg

[5]. Brain  image with tumor Available from: 
https://upload.wikimedia.org/wikipedia/commons/thumb/5/5f/Hirnmetastase_MRT-T1_KM.jpg/300px-Hirnmetastase_MRT-T1_KM.jpg

[6]. Tonmoy Hossain, Fairuz Shadmani Shishir, Mohsena Ashraf
MD Abdullah Al Nasim &, Faisal Muhammad Shah5$ Brain Tumor detection using Convolutional Neural network Proceedings of the IEEE conference on computer vision and pattern recognition, 2019.

[7]. Suhib Irsheidat, Rehab Duwairi  Brain Tumor Detection UsingArtificial Convolutional Neural Networks Proceedings of the IEEE conference on computer vision and pattern recognition, 2020.

[8]. Pankaj Sapra, Rupinderpal Singh, Shivani KhuranaBrain Tumor Detection Using Neural Network Proceedings of the IEEE conference on computer vision and pattern recognition, 2013.


[9]. Hassan Ali Khan, Wu Jue, Muhammad Mushtaq  and Muhammad Umer Mushtaq Brain tumor classification in MRI image using convolutional neural network Proceedings of the IEEE conference on computer vision and pattern recognition, 2020.

[10].flowcharthttps://www.researchgate.net/profile/Umar-Alqasemi/publication/339786421/figure/fig1/AS:866974074687489@1583714135664/Flowchart-of-Proposed-CAD-System-for-Brain-Tumor-Detection-and-Classification.ppm


[11]. Convolutional Neural Network Image
https://media.springernature.com/lw685/springerstatic/image/art%3A10.1186%2Fs13244-020-00869-4/MediaObjects/13244_2020_869_Fig4_HTML.png

[12]. Pankaj Sapra, Rupinderpal Singh, Shivani KhuranaBrain Tumor Detection Using Neural Network Proceedings of the IEEE conference on computer vision and pattern recognition, 2013.







https://devpost.com/software/glioai-automatic-mri-brain-tumor-detection



