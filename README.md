# MindBigData_MindWaves_Classification_NN
This project requires experimentation with data and classifiers to see what best suits to distinguish between the sequence of brain signals to predict right outcome using Deep Neural Networks. The data consists of brainwave signals of 2sec length avg. each corresponding to one of the 11 total classes -1 to 9, -1 tells not a number and 0 to 9 specifies the digits. 
This dataset is to be classified for 2 major classifications i.e. 
  1. Whether someone is thinking about a digit or not. 
  2. Which exact digit a person is thinking of if thinking of a digit. 
Previous work Previous Work on this dataset shows a maximum accuracy of 30 to 33% using all of provided dataSets with following lines mentioned in them. “The stimulus is a digit from 0–9. Brain signals are captured when the participant sees and thinks about the exposed stimuli. The data has been captured using Muse headband consisting of 4 channels. Some EEG signals were also captured on random actions and labelled as -1. The brain signals are captured over a course of two years from a single test subject. The reported state of the art accuracy for this dataset is 31.35% [30] for 11-class (0–9 or -1) classification and 98% for binary classification (digit or not).” 
I’m currently using 1-D CNN with a batch size of 256 elements with average pooling and at final stages Dense NN with relu as activation function and adam optimizer. This best accuracy achieved by this NN varies between 26-27% whereas accuracy for binary classification varies between 92-95%.The Dataset used for my work only comprises of MindWaves Signals "1 Channel rather than 4 channels" from MindBigData Dataset http://mindbigdata.com/opendb/index.html  
FOR BEST time performance during learning use Keras_GPU library
# Download the dataset from the link given below and place it in src directory named as "MW.txt"
http://mindbigdata.com/opendb/MindBigData-MW-v1.0.zip
