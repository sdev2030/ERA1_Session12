# ERA1_Session12
## Assignment
    1. Move your S10 assignment to Lightning first and then to Spaces such that: 
        1. (You have retrained your model on Lightning) 
        2. You are using Gradio 
        3. Your spaces app has these features: 
            1. ask the user whether he/she wants to see GradCAM images and how many, and from which layer, allow opacity change as well 
            2. ask whether he/she wants to view misclassified images, and how many 
            3. allow users to upload new images, as well as provide 10 example images 
            4. ask how many top classes are to be shown (make sure the user cannot enter more than 10) 
        4. Add the full details on what your App is doing to Spaces README  

## Solution - Notebook [s12_assignment](https://github.com/sdev2030/ERA1_Session12/blob/main/s12_assignment.ipynb)
In this we will use Custom architecture from assignment 10 trained in torch lightning to achieve target test accuracy of more than 90% from the 19th epoch.

Following are the model parameter, train and test accuracies achieved in training the model for 24 epochs.
- Model Parameters - 11,173,062
- Train Accuracy - 96.04%
- Test Accuracy - 92.24%

Graph showing learning rate used in one cycle LR policy.
![LR finder Graph](https://github.com/sdev2030/ERA1_Session12/blob/main/images/onecycle_lr.png)

Graphs from training showing loss and accuracy for train and test datasets
![Training Graphs](https://github.com/sdev2030/ERA1_Session12/blob/main/images/training_graphs.png)

Ten misclassified images from the trained model.
![Misclassied images](https://github.com/sdev2030/ERA1_Session12/blob/main/images/wrong_classified.png)

Gradcam on Ten misclassified images from the trained model.
![Misclassied images](https://github.com/sdev2030/ERA1_Session12/blob/main/images/gradcam_wrong_classified.png)
