# Brain Tumor Detection using Transfer Learning

### Problem Statement:

The goal of this project is to detect brain tumors in MRI scans using transfer learning techniques. The dataset used for this task is the "Brain MRI Images for Brain Tumor Detection" dataset, which consists of MRI scans classified into two classes:

- Class 0: No tumor (encoded as 0)
- Class 1: Tumor present (encoded as 1)

### Dataset Description:

The dataset contains MRI images of the brain, with each image labeled as either having no tumor or having a tumor. The images are grayscale and vary in size.

### Evaluation Metrics:

The performance of the fine-tuned models was assessed using the following evaluation metrics:

- Loss: Binary cross-entropy loss was used as the loss function.
- Accuracy: The percentage of correctly classified images.
- Precision: The ratio of correctly predicted positive observations to the total predicted positive observations.
- Recall: The ratio of correctly predicted positive observations to the all observations in actual class.
- F1 Score: The weighted average of Precision and Recall.

### Findings and Discussion:

| Model       | Accuracy | Loss   | Precision | Recall | F1 Score |
| ----------- | -------- | ------ | --------- | ------ | -------- |
| VGG16       | 0.8812   | 0.2755 |           |        |          |
| ResNet50    | 0.7673   | 0.4555 |           |        |          |
| InceptionV3 | 0.9950   | 0.0404 |           |        |          |

- VGG16: Achieved an accuracy of 88.12%, showing good performance in classifying brain tumor images. Its simple architecture and good performance make it a suitable choice for this task.
- ResNet50: Achieved an accuracy of 76.73%, indicating acceptable performance. Its deeper architecture allows it to capture complex features, which can be beneficial in analyzing medical images.
- InceptionV3: Achieved the highest accuracy of 99.50%, showing excellent performance. Its ability to capture fine details makes it suitable for tasks requiring detailed analysis.

### Strengths of Transfer Learning:

- Transfer learning allows us to leverage the pre-trained models' weights, reducing the need for large amounts of labeled data and training time.
- It enables the use of state-of-the-art architectures and techniques, which can improve performance.

### Limitations of Transfer Learning:

- Pre-trained models may not always generalize well to new domains, requiring fine-tuning and adaptation.
- The choice of pre-trained model and the extent of fine-tuning can significantly impact performance.
