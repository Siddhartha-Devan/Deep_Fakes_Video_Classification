This project is an attempt to identify deepfake videos. I have used 300 videos from celeb-df dataset to build a classification model.

The model is based on conv3d layers. I have also tried a convlstm model which gave a very low accuracy. 

In the first step of preprocessing, I cut out the head and its surrounding regions from the complete video using mediapipe face recognition. 

To train the model, I have only used the first 20 frames to check if a video is deepfake or original (I should have used atleast 50) due to limited computational power in my pc. (4gb gtx 1650)

