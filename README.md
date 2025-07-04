# Language-Translator
This is a Python script that uses several libraries to perform speech-to-text translation, text translation, and text-to-speech synthesis. Here's a breakdown of what each part of the code does:

1. The **`googletrans`** library is imported for text translation, **`speech_recognition`** for speech recognition, **`gtts`** for text-to-speech synthesis, **`playsound`** for playing audio files, and **`time`** for adding delays.
2. The input and output languages are set to English and German, respectively.
3. A **`Recognizer`** object is created from the **`speech_recognition`** library to recognize speech.
4. The user is prompted to choose an option: translate from audio or translate from text.
5. If the user chooses option 1 (translate from audio), the script uses the microphone to record audio for up to 5 seconds. The recorded audio is then recognized as text using the **`recognize_google`** method.
6. If the user chooses option 2 (translate from text), the script prompts the user to enter the text to translate.
7. The **`Translator`** object from the **`googletrans`** library is used to translate the text to the output language.
8. The translated text is then converted to audio using the **`gTTS`** (Google Text-to-Speech) function from the **`gtts`** library.
9. The converted audio is saved as an MP3 file named "hello.mp3".
10. Finally, the **`playsound`** function is used to play the converted audio.

In summary, this script allows the user to translate speech or text from English to German and plays the translated text as audio.
