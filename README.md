# sound-project
This code demonstrates a basic example of audio recording, filtering, and speech recognition in Python.


This Python code performs audio recording using PyAudio, filters the recorded audio using a bandpass filter, and then performs speech recognition on the filtered audio. Here's a breakdown of what each part of the code does:

Recording Audio:

It uses PyAudio to open an audio stream and record audio for 5 seconds.
The recorded audio is stored in a list called frames.
Filtering Audio:

It reads the recorded audio from the file 'record.wav'.
A bandpass filter is applied to the audio data using scipy.signal.butter and scipy.signal.lfilter to filter out frequencies outside the specified range (lowcut to highcut).
The filtered audio is then saved to a new WAV file called 'record_filtered.wav'.
Plotting Audio Signals:

It uses matplotlib to plot the original and filtered audio signals.
Speech Recognition:

It uses the speech_recognition library (recognized as sr) to perform speech recognition on the filtered audio.
The AudioFile class is used to load the audio file.
The recognize_google method is used to recognize speech from the audio file, specifying the language as 'en-US'.
The recognized text is then printed to the console.
