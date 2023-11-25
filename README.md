# Listed-Fans-Company-Assignment-
## Deep Learning &amp; NLP
### Inference:

* The assignment involves creating a voice cloning model that can generate a synthetic voice in a different language while retaining the original speaker's pitch and audio tone.
* The code extracts a text input in one language (e.g., English) and aims to translate it into the target language (e.g., Hindi).
* It then uses a Text-to-Speech (TTS) engine to synthesize the translated text into speech.

# Here's a breakdown of the tasks performed in the code:

## Preprocessing:

The input text is provided in any language (in this case, it's "Hello, this is a sample text to be converted to Hindi").
Language detection is performed using the langdetect library to determine the input language.

## Language Translation:

If the input language is different from the target language (in this case, "hi" for Hindi), translation logic is implemented using the googletrans library to translate the input text.
The translated text is stored in the variable translated_text.

## TTS Engine Selection:

The code selects a Text-to-Speech (TTS) engine using the gTTS library, specifying the target language (Hindi) and setting the speech speed as not slow.

## Synthesis:

The synthesized speech is generated and saved as an audio file named "output.mp3."

## Post-processing:

The code uses the pygame library to initialize the audio mixer and play the generated audio file.
The output speech is saved to a specified path (in this case, 'C:/Users/chenn/Downloads/output.mp3').

## Output:

The code prints a message indicating that the speech has been generated and saved.
