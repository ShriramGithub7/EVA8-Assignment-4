# EVA8-Assignment-4

This repository is ceated to build Convlution Neural Network model in multiple steps like basic structure to advanced level

Below is detailed analysis of target, results and analysis of each of the 3 steps

Step1:
    Target:
      Create basic setup
      Setup transforms, data loader and basic working code
    
    Results:
      Parameters: 2.7M
      Best training Accuracy: 99.92%
      Best Test Accuracy: 99.29%
    
    Analysis:
      Model is working and able to achieve good accuracy but not 99.40%
      Model is quite heavy
      Model is overfitting

Step2:
  Target:
    Change the skeleton to add different blocks like Input, Convolution, Transaction and Output block
    Reduce the size of the model to keep it under 15K
    Add batch normalization to increase model efficiency
    Add regularization, dropout, GAP
  
  Results:
    Parameters: 14.5K
    Best training Accuracy: 99.24%
    Best Test Accuracy: 99.10%%
  
  Analysis:
    Model is made light-weight with parameters under 15k
    Model is overfitting
    Model is far from its expected accuracy of 99.40% as it achieved max 99.10% accuracy

Step3:
  Target:
    Change the input and output channel size
    Add dropout at each layer and also change the value from 0.25 to 0.1
    Add rotation
    Add Learning Rate scheduler
  
  Results:
    Parameters: 9,696
    Best training Accuracy: 98.36%
    Best Test Accuracy: 99.26%
  
  Analysis:
    Model has achied required parameters of under 10k
    Model is underfitting as training accuracy is much less than test accuracy
    Model has consistntly achieved accuracy around 99.25 but not 99.40%


Conclusion:
  Model still needs to be finetuned to achieve test accuracy of 99.40% within 10k parameters and 15 epochs
