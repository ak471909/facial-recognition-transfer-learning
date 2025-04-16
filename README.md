# facial-recognition-transfer-learning
The aim of the project to use transfer learning by implementing an image classification task using Inception models.The focus was specifically on facial recognition, a common application in areas such as airport security and police systems. The goal is to develop a system that can identify individuals from a given set of images, mimicking the facial recognition process used in smart gates at airports.  

**Pre Trained Model**: The model used is MobileNetV2, a CNN deep learning model specifically designed for image classification, object detection, and facial recognition. It is optimized to have a low computational cost by using inverted residuals and linear bottlenecks, making it well-suited for the computing system employed to complete the task. 

https://www.tensorflow.org/api_docs/python/tf/keras/applications/MobileNetV2 

**Dataset**: The task focuses on facial recognition, so the dataset used to fine-tune the pre-trained model is selected accordingly. The dataset chosen for this purpose is the Celebrity Faces Dataset from Kaggle because it allows for classifying individual celebrities based on their facial features. If the model achieves high accuracy when fine-tuned to this dataset, the learned knowledge should be transferable to a different set of faces, such as a criminal dataset for police applications. 

https://www.kaggle.com/datasets/vishesh1412/celebrity-face-image-dataset 

**Why use transfer learning**: 
Transfer learning is ideal for this task because it allows the use of a pre-trained model, like MobileNetV2, which already understands basic features from a large dataset. Instead of starting from scratch, the model can be quickly fine-tuned on the smaller Celebrity Faces Dataset.  The advantages of applying transfer learning to our task include faster training, as pre-trained models already recognize basic features like eyes and facial contours, reducing the time needed for fine-tuning.  It also requires less data compared to training a model from scratch, which would need millions of images. Transfer learning can achieve accurate results with a smaller dataset. Pre-trained models generalize well to new tasks, and fine-tuning them on specific data improves accuracy.  Additionally, transfer learning lowers computational costs by reusing learned weights and helps prevent overfitting by starting with a strong feature extractor. 


