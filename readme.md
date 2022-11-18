# Dice-Numbers-AI

The documentation for my AI project of detecting what number is rolled on a six sided die.

[Imgur](https://i.imgur.com/3yVYOKy.jpg)

## The Algorithm

The first thing required to create this algorithm is the dataset, a collection of dice rolls ranging from 1 to 6, formatted with training, validation, and testing folders. Then this dataset is run through an unsupervised learning training script where the script looks at the training images, sees connecctions and draws conclusions about the images in each different catagory folder, validates those connections with the validation images, and then finally tests them with the test images. It then takes these connections and turns it into a model that we can run other images into, and get an accurate result.

## Running this project

1. 'cd' into the 'my_project' directory
2. run: 'imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/{folder input file is in}/{input file name}.jpg {output file name}.jpg' and replace the {}'s with what is specified inside of them
3. scp the outputted .jpg file onto your computer or view it by some other means (Ex: VisualStudio)

Required Installed Libraries:
  - torch
  - torchvision

[View a video explanation here](video link)
