# COMP562-Face-Mask-Detect

## Demo

https://youtu.be/d2ylPwF7zrc

<iframe width="560" height="315" src="https://www.youtube.com/embed/d2ylPwF7zrc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

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
<br><br>
The application code is in the notebook in the repo's root directory: [comp562-face-mask-detector.ipynb](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/blob/main/comp562-face-mask-detector.ipynb)
<br><br>
Clone the GitHub repository, and open the notebook using Jupyter Notebook. To use just the app, simply run the **last cell** in the notebook. We have provided our trained PCA-SVM classifier model as a saved pickle object, [face_mask_detect_model.pkl](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/blob/main/face_mask_detect_model.pkl), that will get automatically loaded when you run the **last** cell, if it is kept in the same directory as the [comp562-face-mask-detector.ipynb](https://github.com/aannirajpatel/COMP562-Face-Mask-Detect/blob/main/comp562-face-mask-detector.ipynb) notebook.
<br><br>
If you would also like to train the model, or see how everything works, go in the order from first cell to last!
<br><br>
Please show your love, and leave a like if this helped!

## Troubleshooting

If the app is classifying wrongly, try facing the camera head-on and move closer to the camera. Make sure light is falling onto your face to illuminate it enough.

## References

1. The original MTCNN research paper: https://arxiv.org/abs/1604.02878

2. Face Mask Detection Dataset on Kaggle: https://www.kaggle.com/andrewmvd/face-mask-detection

3. Working of MTCNN: https://towardsdatascience.com/how-does-a-face-detection-program-work-using-neural-networks-17896df8e6ff

4. How to use MTCNN in facenet-pytorch: https://www.kaggle.com/timesler/guide-to-mtcnn-in-facenet-pytorch

5. For learning how to code up a PCA-SVM pipeline: https://jakevdp.github.io/PythonDataScienceHandbook/05.07-support-vector-machines.html

6. For handling the Face-Mask-Detection dataset and creating the <b>data</b> and <b>labels</b> arrays: https://www.kaggle.com/notadithyabhat/face-mask-detector/
