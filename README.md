# Background Music Transcription
This repository provides an automated pipeline to extract background music from YouTube videos and convert it into a textual transcription. The solution leverages widely used tools—yt-dlp for downloading and converting video audio to MP3, and Whisper for transcribing the audio content.

## Prerequisites

Before using the scripts in this repository, make sure you have the following installed and set up:

- **yt-dlp:**  
  [yt-dlp GitHub Repository](https://github.com/yt-dlp/yt-dlp)  
  Used for downloading and converting YouTube video audio.

- **FFmpeg:**  
  Required by yt-dlp for audio extraction:
  ```bash
  sudo apt update && sudo apt install ffmpeg -y
  ```

- **Whisper:**
  Whisper GitHub Repository
  ```bash
  pip install git+https://github.com/openai/whisper.git
  ```

## Key Features

- **YouTube Audio Extraction:**  
  Download audio directly from any YouTube URL and convert it into an MP3 file using `yt-dlp`.

- **Automatic MP3 Detection:**  
  A built-in mechanism automatically searches your working directory for the downloaded MP3 file, ensuring a seamless transition to transcription.

- **Audio-to-Text Transcription:**  
  Convert the extracted MP3 file into text using the Whisper transcription model. You can adjust the model size (e.g., small, medium, large) to balance speed and accuracy.

- **Interactive Google Colab Notebook:**  
  For those who prefer an interactive environment, a complete Colab notebook is provided. This notebook installs the necessary dependencies and guides you through the process from audio extraction to transcription.


