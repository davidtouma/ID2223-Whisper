# ID2223-Whisper-transcriber

In this project, we fine-tune an existing pre-trained transformer model on the Swedish language. The model used was Whisper. This project is divided into mainly two different notebooks, one that handle the feature engineering and saves the dataset (which is multiple GB of data) to Google Colab. The second notebook handles the model pipeline, and trains and upload the fine tuned model. 

Training the model takes around 8 hours depending on hardware and parameters used. Making sure the data is ready takes around 15-20 minutes. For that reason, we the two notebooks are split up and not combined to one. 

The application is a simple UI where we use our transformer model to transcribe. You can simply talk into your microphone and submit your recorded message. The model will then output your recording as text (transcribe)

The app can be found here: https://huggingface.co/spaces/davidt123/Whisper-transcriber-swe


# Task 2 - How to improve the model performance
 Model-centric approach:
 
 Model-centric approaches involves some changes in the hyperparameters of the model. One possibly way of trying this, is to use the Huggingface Trainer API (https://huggingface.co/docs/transformers/hpo_train), where you can set different values of parameters (for example learning rate, per device batch size, etc). This will then go over the different values for the parameters and save the best model (the parameters that provided the best model)
 
 I tried doing this, but were not able to make it work.
 
 Data-centric approach:
 
 A data centric-approach involves doing modification to the data, or perhaps changing to another dataset that could be better suited for the task. Common voice is probably the most commonly used dataset for speach recognition, but there are other datasets one could look at. To find different datasets you can look at https://huggingface.co/datasets?task_categories=task_categories:automatic-speech-recognition&sort=downloads.
