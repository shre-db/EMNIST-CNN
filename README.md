# EMNIST-CNN
![cover](images/EMNIST_cover.png)

Overview
--------
This project involves the use of a Convolutional Neural Network (CNN) to classify handwritten characters in the EMNIST dataset. The EMNIST dataset was gathered using the torchvision library. The CNN architecture includes 3 convolutional layers and 3 fully connected layers. Batch Normalization and Dropout Regularization techniques were applied to both types of layers during the training of the model to improve its performance. The loss and accuracy were measured at each epoch during the training process to evaluate the performance of the model. Finally, the measurements were plotted to visualize the performance of the model. This README file provides an Overview and includes other information related to the project as outlined in the Table of Contents.

Primary Objective
-----------------
To design and implement a Convolutional Neural Network (CNN) that is capable of accurately classifying handwritten characters in the EMNIST dataset. This will be achieved by utilizing the EMNIST dataset gathered through the torchvision library.

Results
-------
Since the dataset was balanced accuracy score was used as the performance measure. On application of Batch Normalization and Dropout Regularization, the trained model was able to achieve a test accuracy of 95.11%.

Usage
-----
If you are looking for a trained model for Transfer Learning or to be able classify the EMNIST images right off the bat, the models folder has a trained CNN called 'EMNISTNet.pt'.

Setup
-----
**prerequisites**
- Google account
- GitHub account
- Git Bash (for Windows)
- Basic understanding of Git and GitHub

If you would like to train a CNN yourself, I recommend [Google Colab](https://colab.research.google.com/). This section provides step by step instructions on establishing connection with GitHub using SSH protocol.
<br><br>
Why is this necessary?<br>Training Deep Learning models are computationally intensive, consequently people utilize GPUs in addition to CPUs for faster execution of the task. If you do not have household GPUs, you can make use of resources provided by cloud services like Google Colab, AWS, Azure or others. That said, there are limitations to the usage of these resources. You can find out more about Google Colab through the link provided above.
<br>
<br>
Let's kick things off by breifly describing the procedure.
The Idea is to setup local repository on your Google Drive and then use SSH protocol to interact with a remote repository (GitHub).
To do this you need a Secure Shell (SSH) key pair. This key pair has a public and a private key. The key pair can be generated using Git Bash (for Windows) or Terminal (Mac or Linux) or even on Google Colab's code cells with a '!' sign preceeding commands. The private key is then stored on your Google Drive and the public key on GitHub. The next step is to add the private key to an SSH agent. SSH agents provide a secure and efficient way to manage and use SSH keys for remote authentication.

1. **Generating SSH key pair**<br>
On your computer open Git Bash or Terminal and then enter the following command.<br>
`ssh-keygen -t rsa -b 4096 -C "email@example.com"` and press Enter.<br>
The default location to save the key is in your user directory in .ssh folder and it will be called 'id_rsa', for example `/Users/Shrey/.ssh/id_rsa`, you can leave it as it is. In the next substep you can optionally enter a pass phrase for your key or leave it blank. Once you are ready press enter. The key pair is generated and stored in the location specified above.
2. **Access the keys**<br>
