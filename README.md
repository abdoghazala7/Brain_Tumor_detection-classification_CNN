# <h1><center>Unified CNN Approach for Multi-Class MRI Brain Tumor Classification<center><h1>

# About Dataset:
>
>- `What is a brain tumor?`
      A brain tumor is a collection, or mass, of abnormal cells in your brain. Your skull, which encloses your brain, is very         rigid. Any growth inside such a restricted space can cause problems. Brain tumors can be cancerous (malignant) or       noncancerous (benign). When benign or malignant tumors grow, they can cause the 
      pressure inside your skull to increase. This can cause brain damage, and it can be life-threatening.
>
>- `The importance of the subject:` Early detection and classification of brain tumors is an important research domain in the field of medical imaging and accordingly helps in selecting the most convenient treatment method to save patients life therefore
>
>
>- `The category of tumor and number in each Training and Testing data:` Training: glioma: 1321 ,meningioma: 1339 ,notumor: 1595
pituitary: 1457
    and  Testing:
             glioma: 300 , meningioma: 306 , notumor: 405 , pituitary: 300

# About Notebook:

>- `Overview:`
>This project aims to classify brain tumor images into four categories: glioma, meningioma, notumor, and pituitary. The classification task is accomplished using transfer learning, where pre-trained convolutional neural network (CNN) models are fine-tuned on the brain tumor dataset.
># `Key Steps:` 
>- `1.Data Exploration:` The dataset consists of images categorized into training and testing sets for each tumor type. The distribution of data across classes is visualized to understand the dataset's composition.
>
>- `2.Data Preprocessing:`Data Preprocessing: Image data is loaded using TensorFlow's image_dataset_from_directory function. Preprocessing steps include resizing images, splitting data into training and validation sets, and applying one-hot encoding to labels.
>
>- `3.Model Selection:`Model Selection: Several pre-trained CNN models, including DenseNet121, VGG16, ResNet50V2, MobileNetV2, EfficientNetV2S, and Xception, are selected for transfer learning. These models are imported from TensorFlow's applications module.
>
>- `4.Fine-Tuning:` The selected pre-trained models are fine-tuned on the brain tumor dataset. The top layers are adapted to the new task, while earlier layers are frozen to retain the pre-trained features.
>
>- `5.Evaluation:` The fine-tuned models are evaluated on the testing dataset to assess their performance. Metrics such as categorical accuracy and loss are calculated, and classification reports are generated to analyze model performance across different classes.
>
>- `6.Data Augmentation:` Data augmentation techniques, such as rotation, zooming, and flipping, are applied to enhance the model's ability to generalize to unseen data. Data augmentation is implemented using TensorFlow's ImageDataGenerator class.
>
># `Results:`
>- The VGG16 model achieved the highest accuracy of 97.64% on the testing dataset.
>
>- Confusion matrices and classification reports provide detailed insights into the model's performance for each tumor type.
>
>- Data augmentation improved model robustness and generalization capabilities, leading to better performance on unseen data.

# Conclusion:
Transfer learning, combined with data augmentation, is an effective approach for brain tumor classification. The project demonstrates the importance of selecting appropriate pre-trained models, fine-tuning strategies, and data augmentation techniques to achieve accurate and reliable classification results.

## Here there is  datasets used and all the models trained: https://drive.google.com/drive/folders/1B6amPzGYuBScGl2G3ph1uH5U66CTfPrZ
