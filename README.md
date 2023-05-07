# Guide to install the necessary software and run the models

## Note: There are two models currently available, the original baseline 6-class model trained on 3,500 images under the main branch with an average accuracy of 93.5%, and an advanced 12-class model with an maximum accuracy of 97.6% located in the "extra" folder, the advanced model was trained on 15,515 images and both models were tested on images provided in the Garbage Data Collection Form by Students.

Contributions and suggestions to improve the models are highly encouraged and welcomed. If you would like to contribute to the project, feel free to submit a pull request or open an issue on the GitHub repository. Your input can help make the models more accurate and efficient in classifying waste items.


1. Install *Python 3.10.10* from https://www.python.org/downloads/release/python-31010/
   
   1.1. Make sure to check the Install PiP checkbox when installing python.

2. Install *Visual Studio Code* from https://code.visualstudio.com/download

3. Install *CUDA* if you have a *NVIDIA GPU* from https://developer.nvidia.com/cuda-downloads and follow the installation instructions. (optional)

4. Install *cuDNN* from https://developer.nvidia.com/cudnn and follow the installation instructions. (optional)

5. Download the repository (Press the green Code dropdown button, and press Download ZIP)

6. Extract the repository to a folder of your choice and open it in Visual Studio Code.
   
   6.1. Open the Command Prompt and type `pip install` [insert module names here] the modules mentioned in the first code cell of the baseline and advanced garbage classifier files.

*Example input for Step 6.1:*
`pip install torch, torchvision, matplotlib, numpy`

7. Open the **garbage_classifier_smam.ipynb** or the larger, more powerful **advanced_garbage_classifier_smam.ipynb** file and run it cell by cell.

8. Train the model, or use the pre-trained **accuracy_96_normal_model.pth** or **original_model** files in the *models* folder, and run the model on the test images (under the visualize predictions sub-heading), or on your own images by adding images to the external folder.

9. Run the `predict_random` function by passing the name of the image **name.jpg** (insert the name of the image in place of "name") as a parameter to the function to predict the class of the image.

*Example input for Step 9:*
`predict_random("name.jpg")`

Note: You may have to change the path of the images in the code to run the model on your own images.
      Steps 3 and 4 are recommended if possible, though optional and will only reduce training times, without any adverse effect on the model.
      Step 1 is mandatory to run the model.
      Step 6.1 will run without error if `pip` installation was proper during Python 3.10.10 installation (Step 1.1)
      
      
      
## This repository is continuously updated and enhanced as new feature improvements become available. Therefore, there may be minor differences in the folders and program files depending on the timing of updates.

#### However, this README file will also be updated periodically to reflect any new changes made to the repository.
      
