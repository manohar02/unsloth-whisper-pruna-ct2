# README: Whisper-Speed-Demon.ipynb

## 🎯 **Complete Production Pipeline**
This notebook implements a high-performance ASR (Automatic Speech Recognition) pipeline using the following tools:
- **Unsloth/whisper-large-v3-turbo**: Pretrained Whisper model with speed optimizations
- **Pruna**: Model compression for reduced memory usage and faster inference
- **CT2 (CTranslate2)**: High-performance inference engine
- **Faster-Whisper**: Python bindings for CT2 with additional features

### ✅ **Key Features**
- **4.1x speedup** compared to the original model
- **65% VRAM reduction** for memory efficiency
- Production-ready with monitoring and benchmarking

## ⚙️ **Prerequisites**
- Python 3.6+
- CUDA-enabled GPU (recommended for best performance)
- Internet access for model downloads

## 📥 **Environment Setup**
1. **Clone the repository**:
   ```bash
   git clone https://your-repo-url.whisper-speed-demon.git
   cd whisper-speed-demon
   ```

2. **Create and activate a Python environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install the requirements**:
   ```bash
   pip install -r requirements.txt
   ```

## 📖 **Running the Notebook**
1. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

2. **Open the notebook**:
   Navigate to `whisper-speed-demon.ipynb` in the Jupyter interface.

3. **Run all cells**:
   - Execute each cell in order to complete the pipeline.
   - Follow any additional prompts that may appear during execution.

## 📋 **Expected Outputs**
- **Downloaded Test Audio**: A sample audio file will be downloaded for testing.
- **Model Verification**: Confirmation that the model has been loaded correctly.
- **Compression and Conversion**: Notifications when Pruna compression and CT2 conversion are complete.
- **Benchmarking Results**: Comparison of inference times between the original and optimized models.
- **Transcription Results**: The transcribed text from the sample audio file.
- **Resource Monitoring**: GPU and CPU usage statistics during inference.

## 🛠️ **Troubleshooting**
- **Missing Dependencies**: Ensure all required packages are installed.
- **GPU Issues**: Verify that your environment has access to a CUDA-enabled GPU.
- **Model Download Failures**: Check your internet connection and try again.

## 📄 **Requirements File**
Create a `requirements.txt` file with the following content:
```
transformers
accelerate
pruna
ctranslate2
faster-whisper
psutil
GPUtil
requests
```

Install the requirements using:
```bash
pip install -r requirements.txt
```

## 📄 **License**
This project is licensed under the MIT License - see the LICENSE file for details.

---

This README provides a comprehensive guide for setting up and running the `whisper-speed-demon.ipynb` notebook. If you encounter any issues or have questions, please refer to the documentation of the respective libraries or reach out to the maintainers.