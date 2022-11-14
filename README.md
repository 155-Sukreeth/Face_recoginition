# Face_recoginition
1) Run 01_collect_data.ipynb file to give input to the model(face capture), this requires allowing the model to install required packages(opencv, numpy etc) and providing acces to your camera.

2) provide one unique number for each person which will be used as the id for that person. Once the camera is active, it will capture 30 images and stores them in the Dataset directory.

3) Once the data is gathered, run the 02_trainer.ipynb file to train the model, once the model is trained it will save the data in .yml format in trainer directory.

4) Now run the 03_recognizer.ipynb file, add your name to the names list for the model to map with your previously provided id. Once the camera is active it will detect the face and predicts the person. It will then display the name of the person and the confidence level of the model at which it makes its predictions (to increase the confidence score, we need to increase our dataset of that particular person).

Note: install necessary packages(opencv-python, opencv-contrib-python, numpy, pillow, matplotlib, pandas), extra code(or web apis) might be needed to allow hardware resources (such as camera) in google collab. If jupyter notebook is being used, ensure your system meets the hardware requirements. 
