# Image-to-Text-to-Explanation Project

Welcome to the Image-to-Text-to-Explanation project repository! This project focuses on converting images into text and providing detailed explanations.

## Overview

This repository contains the code for a system that converts any given image with text to textual representation and explanations based on the identified content.

## Features

- **Image Processing:** Converts the original input image to [BGR image](https://stackoverflow.com/questions/367449/what-exactly-is-bgr-color-space), and [grayscaled image](https://www.vfpresets.com/lightroom-glossary/grayscale/#:~:text=Grayscale%2C%20in%20photography%2C%20is%20a,are%20actually%20not%20the%20same.). 

- **Image-to-Text Conversion:** uses a sophisticated image processing method called *[EasyOCR](https://github.com/JaidedAI/EasyOCR)*, that is based on deep learning to convert the image into written text.

- **Text Processing:** relies on a word-by-word correction method. Uses the [370k English words corpus](https://www.kaggle.com/datasets/ruchi798/part-of-speech-tagging) dataset to compare the extracted text with the words in the dataset and make adjustments as needed.
  
- **Text-to-Explanation Generation:** Employs one of the most powerful text generation APIs, *[OpenAI GPT API](https://rapidapi.com/rphrp1985/api/open-ai21)*, to generate explanations based on the extracted text.

## Software

- The code in the repository was tested with Python 3.11.4.

- The packages I used to run the code in this project are listed in [packages.txt](packages.txt) . To install the requirements using The standard package manager for Python *PIP*, run the following at the Terminal command (if you are running JUPYTER notebook on VSCode).

```
pip install InsertThePackageNameHere
