Task 3 (CV)

Video of Model in Action : https://drive.google.com/file/d/1PMttM9RPwO-T6KlsulWB_xa9_aijPPmw/view?usp=sharing

Approach : 
Fisrtly , I imported face images from UTKface dataset which is labelled with 0 & 1 for male and female respectively ,then i preprocessed the images ,Using a res10 dnn face recognition model I got the coordinates of the Face Box,Then I cropped the upper half of the image
which is basically the upper half of the face detected.Then I Made a CNN model which I trained with the processed image data and the label data (that i extracted from the filename).
Next I defined a function for predicting gender with input paramenters as given image , then i preprocessed the given image as i did previously using the same model ,then using the CNN model ,I predicted the label
of the given image i.e. gender .
Additionally I did get some faced masked datasets , of which i labelled 139 manually and then made a func which took input as the directory location of the labelled masked dataset and return accuracy of the model
on the given data.
Additionally,I did gradio implementation in the code which is working fine.

UTKFaceDataset: https://drive.google.com/drive/folders/1HROmgviy4jUUUaCdvvrQ8PcqtNg2jn3G

Labelled masked dataset: https://drive.google.com/drive/folders/1gLja4-Ns2htYzSrJswXaawB5y5jf4pJG?usp=sharing

Saved Model (Weights) : https://drive.google.com/file/d/1sFrkPs4zpB49JW0iV-yZAfs10BQON91t/view?usp=sharing



