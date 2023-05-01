# intro_deep_learning_week3

This is a GitHub repository for a project that aims to identify metastatic cancer in small image patches extracted from larger digital pathology scans using deep learning. The modified version of the PatchCamelyon (PCam) benchmark dataset was used to train and test the algorithm. The goal of the project was to accurately classify images as either containing or not containing metastatic cancer based on the presence of tumor tissue in the center 32x32px region of the image patch.

The dataset provided for classification comprised numerous small pathology images, each labeled with an image ID. The ground truth for the images in the train folder was provided in the train_labels.csv file. The objective was to predict the labels for the images in the test folder. A positive label indicated that the central 32x32px area of a patch contained at least one pixel of tumor tissue.

The deep network used had 3 blocks of convolutions, with each block containing 3 layers. Each block was connected by Maxpooling and Dropout. The model performed well in predicting the classes with an overall accuracy of 92%. The precision, recall, and F1-score for both classes were also high, indicating a good balance between false positives and false negatives. The macro average and weighted average of these metrics were also high and equal, indicating a good balance of the class distribution. Therefore, it can be concluded that the model is performing well in predicting the classes and has a good balance between precision and recall.

Data source: <https://www.kaggle.com/competitions/histopathologic-cancer-detection/data>
