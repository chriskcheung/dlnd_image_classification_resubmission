# dlnd_image_classification_resubmission
udacity - deep learning project 2 Image Classification Resubmission
Problem in 1st submission - accuracy hanging at 10% and not being able to grow further

Problem found to be in conv_net function where 3 layers of convolution and max pool layers were applied. 
The 3rd layers seem to cap size the accuracy. This resubmission uses 2 layers of conv2d_maxpool instead and 
changes to use truncated_random instead of random_normal to add standard deviation control to improve training
This version results in 58% accuracy comparing to 10% accuracy from the original submission.
