# Listed-Fans-Company-Assignment-
## Deep Learning &amp; NLP
### Inference:

* The assignment involves creating a voice cloning model that can generate a synthetic voice in a different language while retaining the original speaker's pitch and audio tone.
* The code extracts a text input in one language (e.g., English) and aims to translate it into the target language (e.g., Hindi).
* It then uses a Text-to-Speech (TTS) engine to synthesize the translated text into speech.

**#Prerequisites**
Make sure you have the following dependencies installed:
Python 3.x
gtts
langdetect
googletrans==4.0.0-rc1
pygame

You can install these dependencies using the following command:
pip install gtts langdetect googletrans==4.0.0-rc1 pygame

**Running the Model**
Clone the repository to your local machine:

git clone <repository_url>
cd <repository_folder>
Open a terminal or command prompt and navigate to the cloned repository.
Edit the input_text variable in the provided script with the desired input text in any language.

Run the script using the following command:
python voice_cloning_model.py
Model Workflow

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

**Evaluating Performance**

Performance evaluation of the voice cloning model can be subjective and may involve listening to the generated speech to assess how well it captures the original speaker's voice in the target language.

Consider the following criteria for evaluation:

Naturalness: How natural does the synthetic speech sound in the target language?
Pitch and Tone: Does the synthesized voice maintain the pitch and tone of the original speaker?
Intelligibility: Is the generated speech clear and intelligible in the target language?
