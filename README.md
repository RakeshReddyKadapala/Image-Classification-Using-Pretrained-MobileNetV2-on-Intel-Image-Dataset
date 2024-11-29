# Image-Classification-Using-Pretrained-MobileNetV2-on-Intel-Image-Dataset
Multi Image classification using tensorflow


transforms--->Compose chains multiple transformations for preprocessing (Resize, Normalize)
The dataset is then divided into training and testing sets, and DataLoader is utilized to streamline the loading process.
MobileNetV2---> a lightweight, efficient convolutional neural network
The training process optimizes the model's parameters using the Adam optimizer and cross-entropy loss. The loop runs for a set number of epochs, during which the model's performance on the training data is iteratively improved.
Finally  classified individual images from the dataset. It showcases how the trained model can make predictions by loading and transforming sample images. 

pred = torch.max(output, 1)
    print(f"Image: {img_path} | Predicted: {train_dataset.classes[pred.item()]}")
