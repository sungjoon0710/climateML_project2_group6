# Topic: Improving the parameterization vertical mixing in the ocean surface boundary layer using a bidirectional long short-term memory neural networl

## Project 2, Team #6

There are no dependencies besides those of the original starter code. 

All data should be precomputed and present in the data folder.

Visualization of Initial Model (2fc) vs Final Model (LSTM-Bi): </link>https://docs.google.com/presentation/d/1A7AaQA6_y3JIf1RZ-5hNoQC-CKxzVdPtN1Sg7DmRMs4/edit?usp=sharing<link>


Term: Spring 2025
## Team members

**Ian Shuman**
**Sungjoon Park**
**Alessandro Castillo**

Project Summary: In this project, we attempt to improve on the first Multilayer Perceptron (MLP) neural network used by Sane et al.’s 2023 paper “Parameterizing vertical mixing coefficients in the ocean surface boundary layer using neural networks” to predict the shape function of vertical diffusivity in the ocean. We do this by altering the architecture of the neural network and by optimizing the model with different activation functions, batch normalization techniques, node-specific weights, and learning rates. Ultimately, a bidirectional long short-term memory model with a tanh activation function, node-specific weights from adaptive optimization, and weight decay was the best performing model. This new model improved the validation loss from ~0.05 to <0.03 and reduced the error around a few, bimodal output nodes, resulting in a dramatic improvement in the prediction of the shape function of the vertical diffusivity gradient compared to the orignial MLP model used by Sane et al.


Contribution Statement: All group members contributed to the design of the study. Ian developed code for the adaptive node-specific weighting,  learn-rate scheduler, bidirectional LSTM, and plots of the input features and gradients of the inputs (not used). Ian also wrote the text of this data story. Sungjoon developed code for expanding the use of model weights, implementing the LSTM, and plotting the observed and predicted shape functions of vertical diffusivity. Sungjoon also collated the group’s code into a working script for the data story and managed the team’s GitHub. Alessandro developed code for implementing a spatial neural network (not used) and the convolutional neural network. All team members contributed to the GitHub repository and prepared the presentation. All team members approve our work presented in our GitHub repository including this contribution statement.

