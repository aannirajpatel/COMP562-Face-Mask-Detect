# COMP562-Face-Mask-Detect

## About

We used a pre-trained Multi-Task Cascaded Convolutional Neural Network (facenet-pytorch MTCNN) and trained a PCA-SVM pipeline to detect faces in images and then classify them to see whether people in those images are wearing masks.

Fall 2020 COMP562 Project at UNC Chapel Hill

## Dataset

We used the Face Mask Detection dataset on Kaggle: https://www.kaggle.com/andrewmvd/face-mask-detection

## Results
<table>
  <tr>
<td>
1. Without mask:<br>
<img src="https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/raw/main/result-face-no-mask.png" alt="Without mask" title="Without mask" width="200">
</td>
<td>
2. Mask worn incorrectly:<br>
<img src="https://raw.githubusercontent.com/aannirajpatel/COMP562-Face-Mask-Detect/main/result-mask-worn-incorrect.png" alt="Mask worn incorrectly" title="Mask worn incorrectly" width="200">
</td>
<td>
3: With mask:<br>
<img src="https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/raw/main/result-face-with-mask.png" alt="With mask" title="With mask" width="200">
</td>
  </tr>
</table>

## Usage

You will require Python 3 along with the following dependencies installed:
1. [numpy](https://numpy.org/install/)
2. [pandas](https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html#installing-from-pypi)
3. os (standard Python library)
4. re (standard Python library)
5. xml.etree.ElementTree (standard Python library)
6. [scikit-learn](https://scikit-learn.org/stable/install.html)
7. [matplotlib](https://matplotlib.org/3.3.2/users/installing.html)
8. [opencv-python (referred to as cv2 in the code, link is for CPU-only package)](https://pypi.org/project/opencv-python/)
9. [scipy](https://www.scipy.org/install.html)
10. pickle (standard Python library)
11. [pytorch](https://pytorch.org/get-started/locally/)
12. [facenet-pytorch](https://pypi.org/project/facenet-pytorch/)

You will also require [Jupyter Notebook](https://jupyter.org/install)
<br>
The application code is in the Jupyter Notebook in the repo's root directory: [comp562-face-mask-detector.ipynb](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/blob/main/comp562-face-mask-detector.ipynb)
<br>
The model has already been trained. You will need to download the dataset from Kaggle if you would like to train the PCA-SVM pipeline with your own parameters. We have provided the model as a saved pickle object, that will get automatically loaded if it is kept in the same directory as the [comp562-face-mask-detector.ipynb](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/blob/main/comp562-face-mask-detector.ipynb) notebook.
<br>
Once you have ensured the above requirements are satisfied, to use the application, just open the [comp562-face-mask-detector.ipynb](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/blob/main/comp562-face-mask-detector.ipynb) notebook with Jupyter Notebook and run the **last** cell.

## References

1. The original MTCNN research paper: https://arxiv.org/abs/1604.02878

2. Face Mask Detection Dataset on Kaggle: https://www.kaggle.com/andrewmvd/face-mask-detection

3. Working of MTCNN: https://towardsdatascience.com/how-does-a-face-detection-program-work-using-neural-networks-17896df8e6ff

4. How to use MTCNN in facenet-pytorch: https://www.kaggle.com/timesler/guide-to-mtcnn-in-facenet-pytorch

5. For learning how to code up a PCA-SVM pipeline: https://jakevdp.github.io/PythonDataScienceHandbook/05.07-support-vector-machines.html

6. For handling the Face-Mask-Detection dataset and creating the <b>data</b> and <b>labels</b> arrays: https://www.kaggle.com/notadithyabhat/face-mask-detector/
