# Collision warning system
This is a modified version based on https://github.com/AshishGusain17/Vehicle-Warning-Indicator-System to work on following environment
<br />

* Python 3.10
* Windows
* tensorflow 2.10.1

Credit goes to the original author.

<br />

### Steps

1. Download the model(ex: ssd_inception_v2_coco_2018_01_28) from tensorflow model zoo listed below in references.
2. Include the model inside models folder and change the model_name variable in integrate3.py to match the model name.
3. Download and add label for the relavant model inside project root and add it to the variable PATH_TO_LABELS inside integrate3.py.
4. Add you collision video to the project root and point the cv2.VideoCapture parameter to it in integrate3.py line 285 `cap=cv2.VideoCapture('video.mp4')`
5. Run `python integrate3.py`


### Dependencies required:
* tensorflow 2.10.1
* keras 2.12.0
* protobuf 4.23.2
* tensorboard 2.12.0
* tensorflow-estimator 2.12.0

### References:
<br />

* https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html on how to install TensorFlow Object Detection API
* https://github.com/tensorflow/models/tree/master/research/object_detection/models this link will have all the pre-trained tensorflow models.
* https://github.com/tensorflow/models/tree/master/research/object_detection/data label list for pre-trained models.