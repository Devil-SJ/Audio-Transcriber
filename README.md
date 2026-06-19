# Audio-Transcriber
```md
# AI Audio Transcriber with Sentence-Level Timestamps

A simple AI-powered audio transcription tool built with **faster-whisper** that converts audio files into clean, readable text with automatic sentence-level timestamps.

The project is designed to run on **Google Colab** and uses GPU acceleration for faster transcription performance.

## Features

- 🎙️ Converts audio files into text transcription
- ⚡ Uses `faster-whisper` for fast and accurate speech recognition
- 🧠 Supports Whisper AI models
- ⏱️ Generates timestamped sentences automatically
- 📝 Creates clean line-by-line transcription format
- 📄 Exports transcription as a `.txt` file
- 🚀 Runs easily on Google Colab with GPU support
- 🌍 Supports multiple languages detected automatically
- 🔇 Includes Voice Activity Detection (VAD) to remove unnecessary silence processing

## Output Format

Instead of normal transcription:

```

This is the first sentence. This is the second sentence. This is the third sentence.

```

The program generates:

```

[00:00] This is the first sentence.
[00:03] This is the second sentence.
[00:05] This is the third sentence.

````

This format is useful for:

- YouTube video scripts
- Subtitle preparation
- Podcast transcription
- Research notes
- Content creation workflows

## Technology Used

- Python
- Google Colab
- faster-whisper
- Whisper AI model
- CUDA GPU acceleration

## Installation

Install the required package:

```bash
pip install faster-whisper
````

## How To Use

1. Open the notebook in Google Colab
2. Run the installation cell
3. Upload your audio file
4. Wait for transcription to complete
5. Preview the generated transcript
6. Download the `.txt` file

## Supported Audio Formats

Common formats supported:

* MP3
* WAV
* M4A
* FLAC
* OGG
* Other Whisper-compatible formats

## Model Options

The project uses:

```
medium
```

You can change the model size:

| Model    | Speed    | Accuracy |
| -------- | -------- | -------- |
| tiny     | Fastest  | Lowest   |
| base     | Fast     | Good     |
| small    | Medium   | Better   |
| medium   | Balanced | High     |
| large-v3 | Slowest  | Best     |

For Google Colab GPU:

* `medium` → Recommended
* `large-v3` → Highest accuracy

## Performance

GPU acceleration is recommended.

Example:

* CPU: slower processing
* GPU: significantly faster transcription

The program automatically uses:

```
CUDA + Float16
```

for better performance.

## Limitations

Whisper generates timestamps based on speech segments. The program improves readability by splitting segments into sentences and assigning timestamps.

For professional subtitle-level accuracy, word-level timestamps can be added.

## Future Improvements

Possible upgrades:

* Word-level timestamp accuracy
* SRT subtitle export
* Automatic punctuation correction
* Speaker detection
* Batch audio processing
* Web interface
* YouTube URL transcription

## License

This project is for personal and educational use.

Built using open-source AI tools.

```
```

