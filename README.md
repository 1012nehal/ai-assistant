from gtts import gTTS
import os

text = input("Enter text for Google to speak: ")
tts = gTTS(text=text, lang='en')
tts.save("output.mp3")  # Save the speech to an MP3 file
os.system(" output.mp3")  # Play the MP3 file (requires mpg321 to be installed on your system)
