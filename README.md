# Sound Generation VAE: What is this project ?

The basic purpose of this project is to combine my theoretical knowledge of Variational Autoencoders (vae) and Tensorflow to build a vae with a specialized 
pre-processing pipeline for dealing with sound files (.wav files) and ultimately develop a vae which can produce sound from mel spectograms. 

# What dataset and libraries are used ?

This project makes use of Tensorflow and Keras Functional API for developing the VAE as well as the pre-processing pipeline. The SoundFile, and Librosa libraries
are also used to create different components of the sound pre-processing pipeline. Other than this, the OS and Pickle libraries are used for loading and saving
the model as well as creating folders as needed. The "Free Sound Digits Dataset" is used to train this specific model.

# How to use this program ?

Just download the .ipynb file and ensure that you have an Nvidia GPU available with cuDNN installed on your local system. Please change the file paths for where
the pre-processed, post-processed dataset is stored as well as all the directories where different components of the model and required files are saved. After making
the appropriate edits just run all the cells and the model should be able to learn and generate the audio based on files in your dataset.

# Future Development ?

Currently, I use an implementation of the Griffim-Lim algorithm to obtain sound from the mel spectograms that I generate with my VAE. Due to this, the sound generated
is very robotic and does not account for pitch and modulation in sound. Thus, I'm unable to use this model to generate music like Beethoven, Mozart, etc. I'm trying to get past this obstacle by learning more theory about sound generation and audio signal pre-processing and further develop this project to be effective for more 
refined sound based tasks.
