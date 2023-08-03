# Real-time Audio Captioning

This Python script captures desktop audio and performs real-time speech recognition, displaying the recognized speech as captions in the terminal. The script uses the `pyaudio` library for audio capture and the `speech_recognition` library for speech recognition.

## Prerequisites

Make sure you have the following libraries installed before running the script:

- PyAudio
- SpeechRecognition

You can install the required libraries using pip:

```bash
pip install pyaudio speechrecognition
```

## How to Use

1. Clone this repository to your local machine or download the `main.py` file.
2. Install the required libraries as mentioned in the Prerequisites section.
3. Run the script using Python:

```bash
python main.py
```

4. The script will start capturing audio from your desktop in real-time and display the recognized speech as captions in the terminal.

## Adjusting Voice Activity Detection (Optional)

The script uses `webrtcvad` for voice activity detection. You can adjust the aggressiveness level to control speech detection sensitivity. The aggressiveness level can be set to values between 0 (least aggressive) and 3 (most aggressive).

```python
# Set aggressiveness level (0 to 3) for VAD, adjust as needed
vad.set_mode(3)  # Aggressiveness level: 0 (least aggressive) to 3 (most aggressive)
```

You can experiment with different aggressiveness levels to find the one that works best for your environment.

## Troubleshooting

If you encounter any issues with audio capture or speech recognition, make sure your microphone settings are configured correctly, and the audio data captured by `pyaudio` is in the correct format.

## License

This project is licensed under the [MIT License](LICENSE).