# Guide to install the necessary software and run the model

1. Install Python 3.10.10 from https://www.python.org/downloads/release/python-31010/

2. Install Visual Studio Code from https://code.visualstudio.com/download

3. Install CUDA if you have a NVIDIA GPU from https://developer.nvidia.com/cuda-downloads and follow the installation instructions.

4. Install cuDNN from https://developer.nvidia.com/cudnn and follow the installation instructions.

5. Download the repository from " "

6. Extract the repository to a folder of your choice and open it in Visual Studio Code.

7. Open the garbage_classifier_smam.ipynb file and run it cell by cell.

8. Train the model, or use the pre-trained "model.pth" or "model2.pth" files in the "models" folder, and run the model on the test images, or on your own images by adding images to the external folder.

9. Run the predict_random function by passing the name of the image "name.jpg" as a parameter to the function to predict the class of the image.

Note: You may have to change the path of the images in the code to run the model on your own images.
