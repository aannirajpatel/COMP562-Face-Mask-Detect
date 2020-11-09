# COMP562-Face-Mask-Detect

## About

We used a pre-trained Multi-Task Cascaded Convolutional Neural Network (facenet-pytorch MTCNN) and trained a PCA-SVM pipeline to detect faces in images and then classify them to see whether people in those images are wearing masks.

Fall 2020 COMP562 Project at UNC Chapel Hill

## Dataset

We used the Face Mask Detection dataset on Kaggle: https://www.kaggle.com/andrewmvd/face-mask-detection

## Results

![Without mask](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/raw/main/result-face-no-mask.png "Without mask")

![Mask worn incorrectly](https://raw.githubusercontent.com/aannirajpatel/COMP562-Face-Mask-Detect/main/result-mask-worn-incorrect.png "Mask worn incorrectly")

![With mask](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/raw/main/result-face-with-mask.png "With mask")

## Usage

You will require Python 3 along with the following dependencies installed:
<ol>
<li>[numpy] (https://numpy.org/install/)</li>
<li>[pandas] (https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#installing-from-pypi)</li>
<li>os (standard Python library)</li>
<li>re (standard Python library)</li>
<li>xml.etree.ElementTree (standard Python library)</li>
<li>[scikit-learn] (https://scikit-learn.org/stable/install.html)</li>
<li>[matplotlib] (https://matplotlib.org/3.3.2/users/installing.html)</li>
<li>[opencv-python (referred to as cv2 in the code, link is for CPU-only package)] (https://pypi.org/project/opencv-python/)</li>
<li>[scipy] (https://www.scipy.org/install.html)</li>
<li>pickle (standard Python library)</li>
<li>[pytorch] (https://pytorch.org/get-started/locally/)</li>
<li>[facenet-pytorch] (https://pypi.org/project/facenet-pytorch/)</li>
</ol>

You will also require Jupyter Notebook

## References

1. The original MTCNN research paper: https://arxiv.org/abs/1604.02878

2. Face Mask Detection Dataset on Kaggle: https://www.kaggle.com/andrewmvd/face-mask-detection

3. Working of MTCNN: https://towardsdatascience.com/how-does-a-face-detection-program-work-using-neural-networks-17896df8e6ff

4. How to use MTCNN in facenet-pytorch: https://www.kaggle.com/timesler/guide-to-mtcnn-in-facenet-pytorch

5. For learning how to code up a PCA-SVM pipeline: https://jakevdp.github.io/PythonDataScienceHandbook/05.07-support-vector-machines.html

6. For handling the Face-Mask-Detection dataset and creating the <b>data</b> and <b>labels</b> arrays: https://www.kaggle.com/notadithyabhat/face-mask-detector/
