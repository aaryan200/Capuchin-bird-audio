# Capuchin-bird-audio
Deep Learning model to count the number of Capuchin bird calls in an audio file
<br>
Dataset used - https://www.kaggle.com/datasets/kenjee/z-by-hp-unlocked-challenge-3-signal-processing
## Steps involved
* Determine the average length of one call of Capuchin bird
* Convert every training data audio file (each training file is a audio file of from 2s to 5s length) to length of average length of one call, which comes out to be approx. 48,000 steps (3s of audio)
* Convert audio files to spectrograms and visualize them
* Create training and testing partitions of dataset
* Build deep learning model and train on training data
* To predict from big audio files of about , convert those clips into windowed spectrograms. Windows are non overlapping, with a length of 48,000 each.
* Pass the windows through deep learning model and count the number of times the model predicts the bird call with a probability of more than 0.99
