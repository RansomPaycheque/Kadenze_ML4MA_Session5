# Kadenze_ML4MA_Session5
Kadenze_Machine_Learning_for_Musicians_and_Artists_Session5


This MFCC feature extractor is a Max 7 patch and relies on the zsa.descriptors_1.01 package, included in this directory.
Before running the patch, copy the above zsa.descriptors_1.01 folder in Max Packages folder, which normally lived in /Documents.
It is meant for the Kadenze mooc Machine Learning for Musician and Artist, by Rebecca Fiebrink. Session 5.
It should successfully help classify music or speech tracks.
I cannot upload anything bigger than 100 MB on here so you will need to download the dataset "gtzan_music_speech" available at: http://marsyasweb.appspot.com/download/data_sets/
This dataset was used for the well known paper in genre classification " Musical genre classification of audio signals " by G. Tzanetakis and P. Cook in IEEE Transactions on Audio and Speech Processing 2002.
In my working directory I have only included the wav versions of both music and speech folders, diminished by 4 samples each.
Concretely, music_wav and speech_wav contain only 60 sample of 30 seconds each instead of 64.
The 8 missing samples are place in a 'test' folder, for testing whether your classification system with Wekinator is doing OK. But you can proceed differently if you wish, you could use all the 64 samples and test with your own…

Steps:

1) Turn on Audio on
2) Drag and drop the music_wav and the speech_wav folder where indicated
3) In Wekinator, open a project with 24 inputs, 1 output, select all classifiers, 2 classes
4) Back in the application, press on 'Music'. Tracks will start to play (I have only limited to 1 second per track but you can change this in the metro object, in edit mode)
5) In Wekinator: select class 1 in output and start recording
6) Wait till 50 something tracks (keeps an eye) then stop recording in Wekinator. Alternatively stop recording (in Wekinator) and press 'stop and reset' in the Application.
7) Repeat from 4) for 'Speech' class
8) After you have recorded sufficient samples, train the model with your classifier of choice (try a few...)
9) Now you are ready to test: drag and drop 'test' folder in Application where indicated, select a track and press Run in Wekinator.
10) Check how your classifier is doing.
