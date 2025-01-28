# ReadMe

## Pre-Requisites
  - Have the entire London_UK folder and the same folder structure

## Instructions on how to run the model
  - Firstly, run the trainer notebook. This will create the folder structure for the manually classified images, from which the model will train.
  - The trainer then outputs a *.pth* file which will be used by the main notebook.
  - Run the main notebook, this will evaluate every image associated with each street segment.
  - THe model takes a while to train, depending on the hardware. It is possible to save the results as *.csv* file to later be merged with the original streets geodataframe. 
