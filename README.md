This project is an attempt to identify deepfake videos. I have used 300 videos from celeb-df dataset to build a classification model.

The model is based on conv3d layers. I have also tried a convlstm model which gave a very low accuracy. 

In the first step of preprocessing, I cut out the head and its surrounding regions from the complete video using mediapipe face recognition. 

To train the model, I have only used the first 50 frames to check if a video is deepfake or original (even frames of first hundred... should have used more) due to limited computational power in my pc. (4gb gtx 1650)

I have also deployed the model in Streamlit and you can try it from the below link:
https://deepfakesvideoclassification.streamlit.app/
