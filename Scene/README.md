**Introduction**

This project is designed for analyzing and classifying environments using multimodal data (images and audio). It was implemented in Jupyter Notebook to provide an interactive environment for data analysis and visualization. The main goal is to demonstrate the potential of the multimodal approach in improving classification accuracy compared to using only one type of data (images or audio).

**About the Dataset**

**Data Source**

The dataset consists of images obtained from 8 different types of environments, along with audio files corresponding to these images. The data was extracted from 37 video recordings, with each second of video represented by an image and MFCC (Mel-Frequency Cepstral Coefficients) statistics for the corresponding audio fragment.

**Key Points:**

Images are extracted at 1-second intervals (frames at 0.5s, 1.5s, 2.5s, and so on).

Each image is accompanied by a set of MFCC audio attributes calculated for the corresponding second of video.

**Problem Statement**

Video from London: The visual classifier incorrectly identifies the environment as "FOREST" when a woman with flowing hair walks by.

Video from Las Vegas: The audio classifier confuses "CITY" with "RIVER" due to the sound of a large fountain.

Solution: A multimodal approach helps eliminate such errors by combining image and audio data.

**Data Format**

Data is provided in the file dataset.csv.

Each row contains:

Path to the image.

104 MFCC attributes derived from audio (13 coefficients across 8 time windows).

Additional Information: The dataset includes two classes for classification:

Class 1: Binary classification - "Indoors" or "Outdoors".

Class 2: Multiclass classification (8 types of environments).

**Project Objectives**

Investigate the impact of the multimodal approach on environment classification.

Explore data characteristics and demonstrate steps for analysis and preparation.

Develop a classification methodology using images, audio, and their combination.

**Technologies Used**

Programming Language: Python.

Development Environment: Jupyter Notebook.

Libraries: Pandas, NumPy, Matplotlib, Scikit-learn, and others.

Project Structure

Data Loading and Preliminary Analysis: Analyze data format and visualize class distribution.

Image Processing: Preprocess and prepare image data for training.

Audio Data Processing: Analyze MFCC attributes, normalize and prepare data.

Multimodal Classification: Combine image and audio data for building classification models.

Evaluation of Results: Compare classification accuracy using single data types and the multimodal approach.

**Citation**

https://www.kaggle.com/datasets/birdy654/scene-classification-images-and-audio/

**Conclusion**

This project demonstrates how a multimodal approach can enhance environment classification accuracy by addressing errors common in single-method classifiers. You can adapt this approach for other tasks and datasets involving multimodal research.