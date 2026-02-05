🖼️ Image Caption Generator with Deep Learning

📋 Project Description:

--> A sophisticated deep learning model that generates descriptive captions for images using a CNN-LSTM architecture. This project implements a complete pipeline for automatic image captioning, combining VGG16 for feature extraction with an LSTM-based decoder for caption generation.

🚀 Key Features:

--> Multi-Modal Architecture: Combines CNN (VGG16) for image understanding with LSTM for sequential text generation

--> End-to-End Pipeline: Complete workflow from data preprocessing to model training and caption generation

--> Transfer Learning: Leverages pre-trained VGG16 for robust image feature extraction

--> Flickr8K Dataset: Trained on the popular Flickr8K image captioning dataset

🏗️ Model Architecture: 

1. Encoder (VGG16):

--> Pre-trained VGG16 (without final classification layer)

--> Extracts 4096-dimensional feature vectors from images

--> Image preprocessing with VGG-specific normalization

2. Decoder (LSTM + Dense Layers):

--> Embedding layer for word vectorization

--> LSTM layer for sequence modeling

--> Dense layers for caption generation

--> Softmax output layer over vocabulary

🛠️ Technology Stack:

--> Deep Learning: TensorFlow 2.x, Keras

--> Computer Vision: OpenCV, PIL

--> Natural Language Processing: NLTK

--> Data Processing: NumPy, Pandas

--> Visualization: Matplotlib, Seaborn

📊 Dataset Information:

--> Dataset: Flickr8K

--> Images: 8,091 natural scene images

--> Captions: 5 captions per image (40,455 total)

📈 Training Details:

-----> Preprocessing Steps:

--> Image resizing to 224×224 pixels

--> VGG16-specific preprocessing (RGB to BGR, zero-centering)

--> Caption cleaning (lowercasing, special character removal)

--> Tokenization and sequence padding

--> Train-test split (90%-10%)

-----> Model Training:

--> Optimizer: Adam

--> Loss Function: Categorical Cross-Entropy

--> Vocabulary Size: 11,638 words

--> Max Caption Length: 29 words

--> Batch Size: Configurable

--> Epochs: Early stopping based on validation loss

--> Vocabulary: ~8,500 unique words (after preprocessing)


