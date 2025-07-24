
# Brain Tumor MRI Image Classification Using Deep Learning
The “Brain Tumor MRI Image Classification” project aims to develop an AI-powered deep learning model that classifies MRI brain images into distinct tumor types: glioma, meningioma, pituitary, or no tumor. Leveraging Convolutional Neural Networks (CNNs) and transfer learning, this project empowers medical professionals with a decision-support tool to detect and differentiate brain tumors from radiological images.

The project workflow begins with an in-depth exploration of the dataset, including visual inspections for tumor distribution and class balance. Images are normalized and resized to ensure consistency, followed by data augmentation techniques such as rotation, zoom, and flipping to enhance model generalization.

Two primary modeling strategies are implemented:

Custom CNN Architecture – A model built from scratch using multiple convolution, pooling, dropout, and dense layers to learn patterns from the MRI scans.

Transfer Learning Models – Pretrained architectures such as ResNet50 and EfficientNetB0 are employed with fine-tuned classification layers to leverage learned features from ImageNet.

The models are trained using the TensorFlow/Keras framework, with callbacks like EarlyStopping and ModelCheckpoint to prevent overfitting and retain the best-performing weights. Evaluation metrics such as accuracy, precision, recall, F1-score, and confusion matrix are used to validate performance. Grad-CAM (Gradient-weighted Class Activation Mapping) is also integrated for visual model explainability, highlighting areas of attention in the MRI scans.

The most accurate model is deployed using Streamlit, a lightweight web framework. The final application allows users to upload MRI images and get real-time predictions along with confidence scores and visual heatmaps showing the model’s focus.

This project has practical applications in healthcare such as AI-assisted diagnosis, triaging of high-risk patients, second-opinion diagnostics in rural areas, and aiding research/clinical trials. It demonstrates the real-world impact of deep learning in life-saving domains, combining technical sophistication with human-centered design.

