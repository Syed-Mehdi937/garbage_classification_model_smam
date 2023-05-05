# Guide to install the necessary software and run the model

## Note: There are two models currently available, the original baseline 6-class model trained on 3,500 images under the main branch, and an advanced 12-class model in the "extra" folder under the main branch, the advanced model was trained on 15,515 images and both models were tested on images provided in the Garbage Data Collection Form by Students.

1. Install *Python 3.10.10* from https://www.python.org/downloads/release/python-31010/
   
   1.1. Make sure to check the Install PiP checkbox when installing python.

2. Install *Visual Studio Code* from https://code.visualstudio.com/download

3. Install *CUDA* if you have a *NVIDIA GPU* from https://developer.nvidia.com/cuda-downloads and follow the installation instructions. (optional)

4. Install *cuDNN* from https://developer.nvidia.com/cudnn and follow the installation instructions. (optional)

5. Download the repository (Press the green Code dropdown button, and press Download ZIP)

6. Extract the repository to a folder of your choice and open it in Visual Studio Code.
   
   6.1. Open the Command Prompt and type `pip install` [insert module names here]' (without the quotes) the modules mentioned in the first code cell (i.e, torch,    matplotlib, os, etc) of the baseline and advanced garbage classifier files.

*Example input for Step 6.1:*
`pip install torch, torchvision, matplotlib, numpy`

7. Open the **garbage_classifier_smam.ipynb** or the larger, more powerful **advanced_garbage_classifier_smam.ipynb** file and run it cell by cell.

8. Train the model, or use the pre-trained "accuracy_96_normal_model.pth" or "original_model" files in the "models" folder, and run the model on the test images (under the visualize predictions sub-heading), or on your own images by adding images to the external folder.

9. Run the `predict_random` function by passing the name of the image "name.jpg" (insert the name of the image in place of "name") as a parameter to the function to predict the class of the image.

*Example input for Step 9:*
`predict_random("name.jpg")`

Note: You may have to change the path of the images in the code to run the model on your own images.
      Steps 3 and 4 are recommended if possible, though optional and will only reduce training times, without any adverse effect on the model.
      Step 1 is mandatory to run the model.
