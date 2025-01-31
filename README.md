# ReadMe

This model uses geotagged streetview imagery and applies a custom convolutional neural network to automatically categorize street segments in a London neighbourhood to a road function and a local amenity. As benchmark and to improve model training accuracy, 406 random images were manually classified based on their observed road function (e.g., pedestrian road) and amenity (e.g., Food & Beverages).

## Pre-Requisites
  - Have the entire London_UK folder (including all images in the imagedb folder) and the same folder structure as specified in the project.

## Instructions on how to run the model
### Run the trainer notebook
  - Open Trainer.ipynb and run all cells. This will:
      - Create the folder structure for the manually classified images.
      - Train the model using the manually classified images.
      - Visualize the accuracy and other validation metrics for the trained models for roads and for amenities.
      - Output a .pth file for roads and for amenities which will be used by the main notebook.
### Run the main notebook
  - Open main.ipynb and run call cells. This will:
      - Evaluate every image associated with each street segment
      - Classify the street segments based on road function and amenities
      - Visualize the results on a map of the London neighbourhood

### Save Results:
The model takes a while to train, depending on the hardware.
It is possible to save the results as a .csv file to later be merged with the original streets geodataframe.
