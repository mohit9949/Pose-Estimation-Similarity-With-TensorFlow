# Pose Estimation Similarity With Tensorflow
This repository consists of all the code required for similar 2-D pose detection in dance videos. This can used for any type of pose estimation application to find the similarity.

We will be using **tensorflow for our position estimation** using openpose for tensorflow.
# Credits:
 **Ildoo Kim**: https://github.com/ildoonet<br>
 GitHub Repo Link: https://github.com/ildoonet/tf-pose-estimation
 
 **Gunjan Seth**: https://github.com/gsethi2409<br>
 GitHub Repo Link: https://github.com/gsethi2409/tf-pose-estimation
### Ipython Notebook File for Pose Estimation Similarity:
```2D-Pose-Similarity.ipynb```
# Requirements:
- Python 3.7
- Tensorflow 2.0+
- OpenCV
# Installation Steps:
 ### 1. Git Clone:
 Clone this repository into your local machine.<br>
 ```git clone https://github.com/mohit9949/Pose-Estimation-Similarity-With-TensorFlow.git```
 ### 2. Installing the requirements:
 Install all the requirements provided in the requirements.txt<br>
 ```cd Pose-Estimation-Similarity-With-TensorFlow```<br>
 ```pip install -r requirements.txt```<br>
 If any problem with downloading pycocotools follow this link at Step 4: https://github.com/markjay4k/Mask-RCNN-series/blob/master/Mask_RCNN%20Install%20Instructions.ipynb
 
 
 ### 3. Install SWIG:
 ```conda install swig```<br>or<br> Download Link: http://www.swig.org/survey.html
 ### 4. Build C++ library for post-processing:
 ```cd tf_pose/pafprocess```
 <br>
 ```swig -python -c++ pafprocess.i && python setup.py build_ext --inplace```
 ### 5. Installing tf_slim:
 ```cd ../../``` <br> 
 ```pip install git+https://github.com/adrianc-a/tf-slim.git@remove_contrib```<br>or<br>
 ```git clone https://github.com/google-research/tf-slim.git```<br>
 and copy the folder ```tf_slim``` in it to our repository ```Pose-Estimation-Similarity-With-TensorFlow```
 ### 6. Download Tensorflow Graph File(pb file).
 ```cd models/graph/cmu```<br>
 ```bash download.sh```<br>
 ```cd ../../..```
 
 
