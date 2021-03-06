# Digit Recognition
## [DATASETS](https://www.openml.org/d/554)
## [ORIGINAL DATA](http://yann.lecun.com/exdb/mnist/)
# Dependencies
1. `cv2`
2. `sklearn`
3. `skimage`
4. `numpy`
5. `collections`

# Contents
This repository contains the following files-

1. `generateClassifier.py` - Python Script to create the classifier file `digits_cls.pkl`.
2. `performRecognition.py` - Python Script to test the classifier.
3. `digits_cls.pkl` - [Classifier file for digit recognition](https://www.researchgate.net/figure/The-learning-process-of-a-classifier-The-classifier-learns-from-the-training-data-The_fig1_333505093).
4. `photo_1.jpg` - Test image number 1 to test the classifier
5. `photo_2.jpg` - Test image numbre 2 to test the classifier

## Usage 

* Clone the repository - 
```bash
cd 
git clone https://github.com/bikz05/digit-recognition.git
cd digit-recognition
```
* The next step is to train the classifier. To do so run the script `generateClassifier.py`. It will produce the classifier named `digits_cls.pkl`. 

**NOTE** - *I have already created the `digits_cls.pkl`, so this step is not necessary.*
```python
python generateClassifier.py
```
* To test the classifier, run the `performRecognition.py` script.
```python
python performRecognition.py -c <path to classifier file> -i <path to test image>
```
ex -
```python
python performRecognition.py -c digits_cls.pkl -i photo_1.jpg
```

## TODO

* Add a CNN Based approach
* Reject bounding boxes lesser than some area
* Look into user errors

## REFERENCES
