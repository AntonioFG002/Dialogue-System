# Dialogue-System

The first thing I did was to create a developer account in TMDB and get the ‘API key’. Then I opened Google Colab with my personal Google account and prepared the audios in the folder ‘/var/Inputs_Audio’, I configured the ‘API_KEY’ in secrets.

Finally, I installed the following in a separate section of the programme 
dependencies: openai-whisper, coqui-tts, tmdbv3api. 

## Audio input

  ➢ I have prepared 4 .wav files by performing the 4 types of queries I have 
  contemplated. These recordings I have made in Praat. 
  
## Audio output
  ➢ At the end of the successful execution of the programme, the generated file in .wav format is automatically downloaded. 
  automatically downloads the generated file in .wav format. 
  
## ASR component
  ➢ I have integrated Whisper so that a particular file is passed to it
  
## Dialogue manager
  ➢ I have extracted the keywords (key information underlined and in bold the 
  movie name) from the user's query. This includes: 
    o The type of information (synopsis, cast, director, score.). 
    o The name of the film (the last two words of the audio). 

  ➢ Interpretation of intentions: 
    o Search synopsis: ‘What is The Godfather about?’ 
    o Search cast: ‘Who are the actors in The Clone Wars?’ 
    o Search for director: ‘Who is the director of The Clone Wars?’ 
    o Search for score: ‘What grade does The Godfather have?’ 

## TTS component:
  ➢ I have used Coqui TTS to convert text (variable response) to audio (audio. 
  ‘answer.wav"): 
