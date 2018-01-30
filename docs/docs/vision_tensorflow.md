# Buoy detection for navigation: Tensorflow approach

## About the classifier
Currently, we've implemented the [Inception-v3 model](https://research.googleblog.com/2016/03/train-your-own-image-classifier-with.html) and retrained the top layer with our own classifiers (buoy, water, sailboats), which returns what the image is most likely to be. With enough data, the classifier should become very accurate and reliable.

## Getting Started
### Pre-Installation
Preferable to run on linux. Contact Irene Chen for a bootable USB to install Ubuntu 17.04.

### Installation of Tensorflow
There's a good official installation guide [here](https://www.tensorflow.org/install/).
Things to note: preferable to set up a virtual environment (virtualenv) to avoid conflicts with python versions.

Starting your virtualenv: 

	source ~/path/to/your/tensorflow/workspace/bin/activate

Common issues: if you've installed python in your virtualenv as well, you could skip this step. If there are conflicts with the python version, manually set up the path.

	export PYTHONPATH=$PYTHONPATH:/path/to/image/classifier/project/lib


## Running the current classifier
Get the entire classifier [here](https://drive.google.com/open?id=11JaHUT94rfeuIKgQn0hfLwjg1EihvNZT) (including the Tensorflow Inception model itself). Can be improved by adding more data in the training_dataset folder.




### Good Reads
