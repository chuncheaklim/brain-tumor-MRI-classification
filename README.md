# brain-tumor-MRI-classification
Multiclassification of different types of brain tumor using deep and transfer learning

In this study, brain tumor MRI images were analyzed using deep and transfer learning techniques to classify them into four tumor types: glioma, meningioma, no tumor, and pituitary. The dataset used for this purpose was obtained from https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset.

Various preprocessing methods were experimented with to observe their impact on model performance. Specifically, two approaches were compared: one involving augmented images, and the other utilizing cropped and augmented images. Surprisingly, there was no significant difference in model performance between these two techniques. Nonetheless, for further investigation, the focus was shifted to the cropped and augmented image approach.

Two neural network models, CNN and ResNet50, were implemented on the dataset. After hyperparameter tuning, the testing accuracy of CNN and ResNet50 reached 98% and 100% respectively. The best combination of hyperparameters was identified through manual tuning, where each parameter was adjusted while keeping the others constant. Although this tuning process required more time for training, it provided more accurate results for comparison with models without hyperparameter tuning. Moreover, this approach successfully resolved the issue of memory crashes that occurred during hyperparameter tuning with GridSearchCV.
