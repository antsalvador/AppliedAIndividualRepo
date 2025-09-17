## Q1 What are the specific problems the team encounters in developing the CNN model for the diagnosis of skin cancer? 

Despite the high effectiveness at identifying skin cancer lesions, CNN models are still prone to mistakes due to the many adversities involved in skin cancer diagnosis. These  challenges include the high variability in skin images due to differences in skin tone, lighting, lesion appearance, and image quality, as well as the complexity and diversity of skin lesions themselves. Models must also cope with class imbalance in datasets—where malignant cases are much rarer than benign ones—and the subtlety of differences between lesion types, which can easily lead to misclassification.

- **Lesion Complexity: Lesions vary in size, color, texture, and border irregularities, making feature extraction and classification difficult.**
- **Dataset Limitations: Many datasets lack diversity, particularly in terms of skin tone, which impacts model inclusiveness and accuracy for underrepresented groups**
- **Image Noise and Preprocessing: Artifacts, poor contrast, and the presence of hair or markings complicate lesion segmentation and diminish model performance.**

#### Relevant links: https://www.liebertpub.com/doi/10.1089/cbr.2024.0161 & https://pmc.ncbi.nlm.nih.gov/articles/PMC11295341/


## Q2 Investigate the concepts of neural networks and machine learning. What are the basic principles of CNNs, and how do they differ from other machine learning techniques? What are the applications and limitations of these technologies in dermatology?

CNNs are specialized neural networks that learn hierarchical representations of spatial data, making them ideal for image analysis such as skin lesion detection. Unlike traditional machine learning methods (e.g., SVM, Random Forest), CNNs automatically extract features rather than relying on hand-crafted descriptors. 

- **Applications: CNNs excel in image classification, lesion segmentation, and prediction of malignancy, often matching dermatologists in image-level diagnosis.**

- **Limitations: Require large, diverse datasets; sensitive to class imbalance and annotation noise; high computational resources; explainability and regulatory concerns in medical use remain significant**

#### Relevant Link: https://arxiv.org/html/2505.21597v1

## Q3 Consider various strategies to enhance the model's accuracy. These could range from optimising hyperparameters to using data augmentation, transfer learning, or integrating additional data such as patient information. Which methods are most suitable for this specific case?

The most promising solution for skin cancer lesion detection is a custom CNN architecture with extensive data augmentation, class weighting to balance training, and inclusion of patient metadata if available. Transfer learning can also be used for rapid prototyping, though a problem-specific CNN may ultimately perform best due to the nuanced nature of skin lesion features. Ethical concerns include ensuring model fairness, preventing bias against underrepresented groups, and ensuring human oversight in final diagnosis.

#### Relevant Links: https://www.liebertpub.com/doi/10.1089/cbr.2024.0161
 
## Select the most promising solution and substantiate this choice with arguments. How will this solution enhance the model's performance? Also consider the ethical implications of using AI in healthcare.

The best solution for this case is a custom CNN architecture, optimized with data augmentation, class weighting, transfer learning for baseline comparison, and integration of patient metadata where available.

- **Task-specific models outperform general ones due to their ability to target dermatological image features.**

- **Augmentation and class weighting counteract dataset imbalance.**

- **Combining patient data and expert feedback increases accuracy and clinical trustworthiness.**

### Ethical Issues:

- **AI in healthcare must be validated thoroughly to prevent diagnostic errors.**

- **Must address biases (e.g., underrepresentation of skin tones) to avoid discriminatory outcomes.**

- **A clinician should always review and interpret model outputs for patient safety.**




## What steps are needed to improve the model? What tools and programming languages will you use? What will the collaboration with dermatologists look like?

## How will the success of the implementation be measured? Which metrics are relevant for assessing the performance of the CNN model, such as accuracy, precision, and recall? How can feedback from doctors be integrated into the evaluation process?

## What have you learned about neural networks, machine learning, and their application in the diagnosis of skin cancer? How has this case contributed to your understanding of the challenges and opportunities within this field?
