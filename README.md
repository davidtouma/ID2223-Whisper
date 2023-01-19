# ID2223-Whisper-transcriber

In this project, we fine-tune an existing pre-trained transformer model on the Swedish language. The model used was Whisper. This project is divided into mainly two different notebooks, one that handle the feature engineering and saves the dataset (which is multiple GB of data) to Google Colab. The second notebook handles the model pipeline, and trains and upload the fine tuned model. 

Training the model takes around 8 hours depending on hardware and parameters used. Making sure the data is ready takes around 15-20 minutes. For that reason, we the two notebooks are split up and not combined to one. 

The application is a simple UI where we use our transformer model to transcribe. You can simply talk into your microphone and submit your recorded message. The model will then output your recording as text (transcribe)

The app can be found here: https://huggingface.co/spaces/davidt123/Whisper-transcriber-swe


# Task 2 - How to improve the model performance
 Model-centric approach:
 
 Data-centric approach:
