# Lizzmotors_assignment
Assignment from Lakshay to Design an End-to-End AI Voice Assistance Pipeline

Recording (5).wav is the audio file that is transcribed by the whisper model before it. The first pre-processing is done in which the sample rate is converted from 48KHz to 16KHz and the audio channel from stereo to mono leading to the creation of a new file named -.

Then from the file, the pseeched part is extracted from the full audio with which the non-speech frame like Background noise, silence is removed leading to a less computation-intensive process sometimes the background noise can also be interpreted as the speech removing this also improves the accuracy.

Then the transcribed text from the audio is extracted and passed into the LLM module - gpt2-medium form which the response to the extracted text query is retrieved and passed to 
the TTS (text to speech) model - parter_tts in which we can adjust the voice type, pitch, and intensity through the normal language manner a the description.

which creates a new audio file is created named - parler_tts_out1.wav.
