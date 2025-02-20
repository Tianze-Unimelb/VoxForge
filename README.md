# VoxForge: Offline Speech-to-Text Tool

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Offline](https://img.shields.io/badge/Works%20Offline-✓-green)
[![Vosk](https://img.shields.io/badge/Powered%20by-Vosk-ff69b4)](https://alphacephei.com/vosk/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

An offline speech recognition tool with real-time audio recording and transcription using Vosk engine, featuring voice activity detection.

## 1. Key Features✨ 
- **100% Offline** - No internet required, all processing done locally
- **Smart VAD** - Voice Activity Detection with adjustable sensitivity
- **Real-time Transcription** - Powered by Vosk's high-accuracy engine
- **Cross-Platform** - Supports Windows/macOS/Linux
- **Lightweight** - Low CPU usage with Python implementation

## 2. Installation 📦 

### Prerequisites
- Python 3.7+
- Microphone

### Install Dependencies 📦 

```bash
# Install required Python packages
pip install pyaudio vosk numpy
```

### Download Model 🌐 
Get Vosk Chinese Model from Baidu Cloud:<br>
🔗 [Download Link](https://pan.baidu.com/s/1UUaPZ4l-xPLOuyJU9tmdXw)<br>
📌 Extraction Code: 6666<br>
Extract model files to model directory

### Quick Start 🚀 
```bash
python main.py
```

### Workflow 🔄 
Start Recording - Press Enter to begin<br>
Speak - (background noise filtered automatically)<br>
Stop Recording - Press Enter again<br>
View Results - Transcribed text appears in console

### Configuration ⚙️ 
Modify parameters in main.py:
```bash
# Silence detection threshold (0-1, default 0.5)
THRESHOLD = 0.5
# Continuous silence frames to stop (default 50 frames≈1s)
THRESHOLDNUM = 50
```

## 3. Sample Output 📄 
*[SYSTEM]* Recording started...<br>
*[RESULT]* 欢迎使用VoxForge离线语音转写工具 (Welcome to VoxForge offline speech transcription)<br>
*[RESULT]* 当前时间是下午3点20分 (Current time is 3:20 PM)<br>
*[SYSTEM]* Silence detected, recording stopped<br>

## 4. Acknowledgements 🙏 
[Vosk](https://alphacephei.com/vosk/) - Efficient offline ASR engine<br>
[PyAudio](https://people.csail.mit.edu/hubert/pyaudio/) - Cross-platform audio I/O<br>
Open-source community contributions<br>
