# Brain-Tumor-Detection-using-CNN
# Abstract :
 A brain tumor is regarded as one of the most competitive diseases among children and adults. The majority of number one Central Nervous System (CNS) malignancies are brain tumors, which account for 85 to 90% of all CNS tumors. Every year, around 11,700 people are diagnosed with a brain tumor. Humans with a malignant mind or CNS tumor have a 5-year survival rate of around 34 percent for men and 36 percent for women. There are three types of brain tumors: start tumor, middle tumor, and end tumor. Malignant Tumor, for example, requires proper treatment, planning, and diagnostics in order to improve the patients' life expectancy. Magnetic Resonance Imaging (MRI) is a great way to detect brain cancers (MRI). 
 
# Introduction :
According to the National Brain Tumor Society, around 700,000 people in the United States have a brain tumor, with the figure rising to 787,000 by 2020 [1]. A brain tumor is not usually more common than other malignancies such as breast cancer or lung cancer, but it is nevertheless the 10th leading cause of death worldwide. Brain cancer is expected to kill 18,020 persons in the next 12 months [2]. A brain tumor has a long-term and mental impact on the lives of those who are affected. A brain tumor develops as a result of tissue damage. An anomaly that develops in the brain or within the main backbone and disrupts normal brain function. There are two types of brain tumors: benign and malignant. Benign brain tumors are benign tumors that do not contain cancer cells and grow slowly. They do not spread and usually live in a single part of the mind, but malignant mental tumors contain cancer cells and develop quickly, spreading to other areas of the mind and backbone. A malignant tumor is both dangerous and life-threatening. The World Health Organization (WHO) has classified brain tumors into grade 1 and 2 low-grade tumors (also known as benign tumors) and grade 3 and 4 high-grade tumors (also known as malignant tumors) based on brain health behavior 

# Objective : 
### Our main objective is to detect a brain tumor from MRI (Magnetic Resonance Image) using CNN (Convolutional Neural Network) .
###
### We developed a model which is able to detect a brain tumor from MRI using CNN , we used a brain MRI data founded on kaggle.
### - The Name of Datasets is 'Dataset Br35H'.
'Dataset Br35H' :   https://www.kaggle.com/ahmedhamada0/brain-tumor-detection
### - The Datasets contain two folder , one is 'yes' and another is 'no'.
### - The folder 'yes' contain MRI that is tumous and 'no' contain non-tumous.
### - We also  used another folder named 'pred' folder , which is used for prediction our model.



## Model and Training
#### The model consists of:

* CNN Layer
* Max Pooling Layer
* Dense Layer
* Fully Connected Layer
* Loss Function: Categorical Cross-Entropy
* Optimization Algorithm: Adam

Model is trained on 20 epochs.

Model | Accuracy | Loss
| :--- | ---: | :---:
CNN Proposed method  | 99.50% | 0.5%

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






