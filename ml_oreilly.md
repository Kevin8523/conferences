# Machine learning O'Reilly

## Chapter 1. The Machine Learning Landscape

Types of ML  <br/> 
* supervised
* unsupervised
* semisupervised
* reinforcement learning

Reinforcement Learning
* agent - observe the environment
* rewards & penalties
* policy - learns by rewards & penalties

Batch Learning
* Must be trained using all the available data
* Also known as offline learning
* Usually done every 24 hours or weekly

Online Learning or Incremental Learning
* Train the system incrementally by feeding it data instances sequentially
* Great for continuous flow data that is needed to adapt to change rapidly or autonomously
* Usually done offline, can be thought of as incremental learning
* Learning rate - Parameter of learning system, how fast should the system adapt to changing data
* Challenge: If bad data is fed into the system, the performance will gradually decline. Need to monitor your system closely and promptly switch learning off if needed.

How do you know which values for your parameters will make your model perform best?
* Specify a performance measure, either:
	- Utility function that measure how good your model is
	- Cost function that measures how bad it is.

Process for modeling in Python with sci-kit-learn
* Import model class
* Instantiate the class and specify the hyper-parameters
* Fit to data
* Apply/predict to new data 

Challenges of Machine Learning
* Insufficient data: Garbage in garbage out

Key Terms:
* Regularization: Constraining a model to make it simplier and reduce the risk of overfitting
* Hyperparemeter: a parameter of a learning algorithim: Used and set prior to training and remains constant during training

Cross validation
* Training set ==> Test Set
* Training set ==> validation set ==> test set (If you want to test parameters)
	+ Training set split into complementary subsets, and each model is trained against a different combination of these subsets and validated against the remaining parts. 
	+ Once th emodel type and hyperparameter have been selected, a final model is trained using these hyperparameters on the full training set, and the generalized error is measured on the test set

