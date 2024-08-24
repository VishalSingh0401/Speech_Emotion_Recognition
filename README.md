# Speech Emotion Recognition

This project involves developing a deep learning model to accurately classify human emotions from speech using the MLPClassifier in Sklearn. The model was trained on the RAVDESS and SAVEE datasets, which together contain over 7,000 audio files representing various emotional states. The objective is to enhance customer sentiment analysis by detecting emotions through speech, which can be applied in various fields such as customer service, mental health, and human-computer interaction.

## Key Features:
- **Datasets**: RAVDESS and SAVEE, consisting of diverse emotional speech recordings.
- **Technologies Used**: Python, Sklearn, Librosa, and other audio processing libraries.
- **Model**: MLPClassifier, designed to process raw audio data and output classified emotions.
- **Applications**: Can be integrated into systems for real-time emotion detection in voice assistants, call centers, and other AI-driven applications.

This repository contains the codebase, datasets (links provided), and instructions for training and testing the model. Contributions and suggestions are welcome!

## How to Use

1. **Download the Datasets**:
   - First, download the RAVDESS and SAVEE datasets from [this Google Drive link](https://drive.google.com/drive/folders/1ghWkRez4EY9j3IdnvS1G3-Da5eNEW47n?usp=sharing).

2. **Place the Dataset Files**:
   - Once all the audio files are downloaded, place the folders named `RAVDESS_Data` and `SAVEE_Data` in the same directory as the `.ipynb` file.

3. **Open the `.ipynb` File**:
   - Open the notebook file in an interpreter such as Jupyter Notebook or Google Colab.

4. **Follow the Comments**:
   - The notebook contains detailed comments in each cell to guide you through the process. Follow these comments to execute the code correctly.

5. **Setup Required Packages**:
   - If the necessary packages are not installed in your environment, uncomment the first cell and run it to install all required dependencies.

6. **Running the Cells**:
   - Run all the cells in the notebook except the last two.

7. **Using the Microphone for Emotion Recognition**:
   - If you want to use your microphone to record your voice for emotion recognition, run the second last cell.

8. **Using a Pre-Recorded Audio File**:
   - If you prefer to use a pre-recorded audio file, run the last cell instead. You may need to tweak the code based on the comments provided:
   ```python
   # Uncomment the following line to use an audio file as an input/Comment the following line to use recording as input
   # new_input = extract_feature("SAVEE_Data\ALL\JK_h01.wav", mfcc = True, chroma = True, mel = True)

   # Comment the following line to use an audio file as an input/Uncomment the following line to use recording as input
   new_input = extract_feature("output.wav", mfcc = True, chroma = True, mel = True)
