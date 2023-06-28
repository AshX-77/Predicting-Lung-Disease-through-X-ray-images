# Predicting-Lung-Disease-through-X-ray-images

Dataset- https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

![image](https://github.com/AshX-77/Predicting-Lung-Disease-through-X-ray-images/assets/120383256/c9548597-ba4c-425d-a3a8-5b00bb50272e)

The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).

Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care.

For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.

Steps to predict if the person has pneumonia or not:
1. Choosing the data set.
2. Importing necessary libraries.
3. Storing the path of training and testing data.
4. Resizing all images to [224,224]
5. Importing the Vgg 16 library as shown below and adding preprocessing layer to the front of VGG
6. Flattening vgg output
7. creating a model
8. compiling the model
9. Using the image data generator to import images from data set
10. Fiiting the model
11. Testing an image from penumonia folder in val ---> correctly predicts pneumonia
