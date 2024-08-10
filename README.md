# Gastro-Intestinal Disease Prediction Using Deep Learning

## Project Overview
This repository hosts the work on predicting gastro-intestinal diseases through image-based machine learning models using the KVASIR dataset. Our goal is to provide non-invasive diagnostics that can enhance medical decision-making and reduce the need for traditional procedures.

## Models Overview
We have implemented multiple deep learning architectures to address the challenges of gastro-intestinal disease classification:

- **VGG16**
- **VGG19**
- **ResNet50**
- **DenseNet121**
- **MobileNet**
- **EfficientNet**

Each model is trained to recognize eight different classes of gastro-intestinal diseases from endoscopic images.

## Model Performance Comparison
The following table summarizes the performance of each model based on accuracy, precision, recall, and mean cross-validation accuracy:

| Model Number | Model Name    | Test Accuracy | Precision | Recall  | Mean Cross-Validation Accuracy |
|--------------|---------------|---------------|-----------|---------|--------------------------------|
| 1            | VGG16         | 83.99%        | 84.41%    | 83.95%  | 81.60%                         |
| 2            | VGG19         | 85.12%        | 85.45%    | 85.63%  | 80.89%                         |
| 3            | RESNET50      | 87.37%        | 87.30%    | 87.25%  | 84.72%                         |
| 4            | DENSENET121   | 90.12%        | 90.30%    | 90.58%  | 85.51%                         |
| 5            | MOBILENET     | 87.66%        | 87.76%    | 87.66%  | 87.32%                         |
| 6            | EFFICIENTNET  | 89.12%        | 89.48%    | 89.26%  | 88.87%                         |

## Key Insights
- **High Correct Predictions:** Models like DenseNet121 and EfficientNet show strong performance in recognizing classes with high accuracy.
- **Confusion in Classification:** Similar visual features between classes like Dyed-Lifted-Polyps and Dyed-Resection-Margins lead to frequent misclassifications.
- **Recommendation:** Improvement in feature extraction and using ensemble methods could potentially increase the accuracy and robustness of the models.
- **Model Specific Strengths:** Each model demonstrates unique strengths in recognizing certain disease classes. For instance, DenseNet121 excels in distinguishing Ulcerative-Colitis, while EfficientNet shows remarkable accuracy in identifying Dyed-Lifted-Polyps. These strengths can be leveraged by deploying specific models based on the prevalence of certain diseases in different clinical settings.

- **Inter-Class Confusion:** The recurrent misclassifications between classes such as Normal-Cecum and Ulcerative-Colitis highlight the need for more discriminative feature learning in these areas. Advanced techniques like attention mechanisms could be incorporated to focus on subtle but critical features that differentiate these conditions.

- **Robustness Across Various Conditions:** While DenseNet121 and EfficientNet provide higher overall accuracies, models like MobileNet demonstrate substantial robustness across different operational conditions due to their architecture, offering a good balance between performance and computational efficiency suitable for mobile or edge computing devices.

- **Impact of Data Augmentation:** Implementing data augmentation strategies such as rotations, scaling, and color adjustments has the potential to reduce overfitting and improve the generalization capability of the models, especially in handling variations within the same disease class.

- **Ensemble Model Potential:** Combining the predictions from multiple models (ensemble methods) could address individual model weaknesses and lead to better overall accuracy. This strategy might be particularly effective in a clinical diagnostic setting where high reliability is critical.

- **Clinical Deployment Considerations:** The practical deployment of these models in a clinical environment would require integration with existing healthcare systems and compliance with medical data regulations. Continuous monitoring and model updating are essential to adapt to new types of data and evolving clinical practices.

- **Future Directions:** Exploring the integration of these models with real-time diagnostic tools and patient management systems could provide comprehensive solutions that extend beyond initial diagnosis to include monitoring and treatment planning.

## Dataset
The models were trained using the KVASIR dataset, which contains 4000 labeled endoscopic images representing various gastro-intestinal conditions.

## Contributions and Acknowledgments
This project is a part of the curriculum for AIT-736-005, conducted by Team Learners. We acknowledge the guidance of Dr. Emanuela Marasco and Mr. Anudeep Vurity. Special thanks to all contributors and the KVASIR dataset providers.

Thank you for exploring our project on GI disease prediction using deep learning!

 
