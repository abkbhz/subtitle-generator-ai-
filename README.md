# subtitle-generator-ai-
1) Live Subtitle Generation
This component utilizes video streaming and performs real-time transcription of the input audio using PyAudio, opencv-python, and Whisper API.
2) Video Subtitle Generation
This component utilizes Deepgram API for high-speed audio transcription, the pyrt library to create subtitles, and the moviepy library for adding subtitles.
Setup
Python libraries
The project is a set of 2 Flask applications that can be run on the localhost after installing the following prerequisites:

deepgram-sdk
moviepy==2.0.0.dev2
imageio==2.25.1
pysrt==1.1.2
flask
openai
pyaudio
opencv-python
Flask-WTF
WTForms
Werkzeug
The above requirements can be installed through the following command:

pip install -r requirements.txt
ImageMagick
The next part of the setup is installing ImageMagick for working on burning subtitles to the video.

We download the binary directly from here and follow steps to install for the respective OS.

OpenAI
We utilize OpenAI's Whisper API for audio transcription. We use this link to set up an OpenAI API key upon creating an account if required.

Deepgram
We use Deepgram API for faster Speech-To-Text audio transcription. We create an account with Deepgram and set up an API key based on this resource.

Once the API keys for OpenAI and Deepgram are created, paste them in the config.py file for the respective variables named OPENAI_API_KEY and DEEPGRAM_API_KEY.

Running the code
To execute the projects, we use the following commands:

Live Subtitle Generation
python live_subtitle_generation.py
Video Subtitle Generation
python video_subtitle_generation.py
