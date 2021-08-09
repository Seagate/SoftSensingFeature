---------
licence by Seagate. 
Please contact: xiaoye.qian@seagate.com, chao.1.zhang@seagate.com, sthitie.e.bom@seagate.com
---------
Deep visualization
---------
Overview:
The project is used for visualizing the deep dilated neural network model. To Understand how the dilated neural network has learned and finetuning the model with the results.

Backgroud and Aim:
The deep visualization translates the information into an understandable context. After implementing a visualization, we are aimed to perform better feature engineering based on the visualization results.

Approach:
The deep visualization approaches are:
1.  Saliency Map
2.  Saliency Map with smooth (add Gaussian noise)
3.  Grad-CAM++
4.  Score-CAM

    Reference:
    Simonyan K, Vedaldi A, Zisserman A. 2014. Deep Inside Convolutional Networks: Visualising Image Classification Models and Saliency Maps.
    
    Chattopadhay, Aditya, et al. "Grad-cam++: Generalized gradient-based visual explanations for deep convolutional networks." 2018 IEEE winter conference on applications of computer vision (WACV). IEEE, 2018.
    
    Wang, Haofan, et al. "Score-CAM: Score-weighted visual explanations for convolutional neural networks." Proceedings of the IEEE/CVF conference on computer vision and pattern recognition workshops. 2020.

Finetuning with the deep visualization results which is including:

*       Adding weighted layer and adjust parameters according to the loss function and backpropagation.
*       Finetuning model focuses on all data. 
*       Finetuning model focuses on partial (misclassified) data. 
*       Finetuning model focuses more on FN data.


# Feature_Selection

To select the features according to the feature importance get from the random forest for every measurement. 

Show the results from:
1. Feature importance of Random forest
2. Shapley Values

Build and validate machine learning model with the high importance selected features:
1. SVM
2. Logistic regression
3. Random forest 
