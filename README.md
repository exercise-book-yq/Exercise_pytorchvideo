# Exercise_pytorchvideo
Running a pre-trained PyTorchVideo classification model using Torch Hub

# Intorduction
PyTorchVideo provides several pretrained models through Torch Hub. In this project I try to load a pre trained video classification model in PyTorchVideo and run it on a test video. The PyTorchVideo Torch Hub models were trained on the Kinetics 400 [1] dataset. Available models are described in model zoo documentation.

# Imports
 First, you should know what packages that you need. 
 
 # Load Model
I select the slowfast_r50 model which was trained on the Kinetics 400 dataset. However, I am confronted a problem that I can't load the model directly from github.
It has http 403 and 404 errors.# Load an example video
We can now test the model with an example video from the Kinetics validation set such as this archery video.

We will load the video and apply the input transform.

# Get model predictions
We can select the numbers of prediction
Therefore, I import the model directly from the pytorchvideo.models.hub.

# Setup Labels
Next I download the id-to-label mapping for the Kinetics 400 dataset on which the torch hub models were trained. This will be used to get the category label names from the predicted class ids.

# Input Transform
Before passing the video into the model we need to apply some input transforms and sample a clip of the correct duration.

NOTE: The input transforms are specific to the model. If you choose a different model than the example in this tutorial, please refer to the code provided in the Torch Hub documentation and copy over the relevant transforms.

For example:
- [SlowFast](https://pytorch.org/hub/facebookresearch_pytorchvideo_slowfast/)
- [X3D](https://pytorch.org/hub/facebookresearch_pytorchvideo_x3d/)
- [Slow](https://pytorch.org/hub/facebookresearch_pytorchvideo_resnet/)

# Load an example video
We can now test the model with an example video from the Kinetics validation set such as this archery video.

We will load the video and apply the input transform.

# Get model predictions
We can select the numbers of prediction

# Evaluate the model
 Efficience and Latency
 evaluate the time of prediction
 
