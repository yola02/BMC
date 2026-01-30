# Bacterial Morphology Classification — Image-Based ML Pipeline

This project focuses on classifying bacterial morphology from microscope images into three categories: cocci, bacilli, and spirilla. The goal is to demonstrate an end-to-end machine learning workflow, from data collection and preprocessing to model training, evaluation, and deployment.

The final model is deployed and shared via Hugging Face, enabling reproducible evaluation and interactive use.

Dataset Overview:

Total images: 600

Classes:

Cocci (200 images)

Bacilli (200 images)

Spirilla (200 images)

Image source: Microscope images collected from web search results

Labels: cocci, bacilli, spirilla

🔗 Dataset link:
https://drive.google.com/drive/folders/1dN3EfDDlfjZP1Yw1RlsErZtNaKafpt-7

Data Collection & Labeling:

Images were collected using automated web scraping tools and manually curated to ensure relevance and quality. Each image was reviewed and labeled based on bacterial shape, a process designed to be fast and consistent given the clear morphological distinctions between classes.

Collection period: September 28, 2024 – October 1, 2024

Labeling approach: Manual labeling based on visual morphology

Modeling Approach:

Used a convolutional neural network with MobileNetV2 as a feature extractor

Applied transfer learning to improve performance on a limited dataset

Evaluated model performance using accuracy and F1 score

Achieved 0.85 accuracy and F1 score on the test set

Tools & Technologies:

Python | TensorFlow / Keras | Pandas, NumPy | Google Colab | Hugging Face (model deployment & sharing)

Deployment:

The trained model is deployed on Hugging Face Spaces, allowing users to upload microscope images and receive predicted bacterial morphology in real time.

This deployment emphasizes reproducibility, accessibility, and practical usability beyond local experimentation.

Key Takeaways:

Demonstrated a complete ML pipeline from raw data collection to deployment

Gained experience applying transfer learning for image classification

Highlighted the importance of data quality, evaluation metrics, and model generalization

Notes:

This project is intended for educational and experimental purposes and focuses on applied machine learning practices rather than clinical diagnosis.
