# AI-Generated-Image-Detector

Simple Streamlit app for detecting whether an image is AI-generated or real using multiple pretrained models.

## Setup

1. Open PowerShell and change to the project folder:
   ```powershell
   cd "E:\New folder\AI-Generated-Image-Detector"
   ```
2. Create a virtual environment:
   ```powershell
   python -m venv .venv
   ```
3. Activate the virtual environment:
   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```
4. Upgrade pip and install dependencies:
   ```powershell
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   ```

## Run

```powershell
streamlit run app.py
```

## Notes

- The app expects pretrained model files in the repository root:
  - `vgg16.h5`
  - `resnet50.h5`
  - `mobilenetv2.h5`
  - `densenet121.h5`
  - `inceptionv3.h5`
  - `efficientnet_b0.pth`
- If a model file is missing, that specific model will fail to load and show a loading error.
- `requirements.txt` is included so the virtual environment can be recreated easily.
