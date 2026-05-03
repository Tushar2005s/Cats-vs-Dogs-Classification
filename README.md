# 🐾 Cat vs Dog Classifier — PROJECT

### Created by Tushar Sharma
**BSc Artificial Intelligence and Data Science**  
**IIT Guwahati**

---

## 📁 Project Files

| File | Purpose |
|---|---|
| `app.py` | Main application code (Streamlit web app) |
| `mobilenetv2.onnx` | Pre-trained AI model (MobileNetV2) |
| `imagenet_classes.txt` | Labels file used by the model |
| `requirements.txt` | Python packages needed |
| `run_app.bat` | Double-click shortcut to run the app (Windows) |
| `.streamlit/config.toml` | App configuration file |

---

## ⚙️ Setup Instructions (Step by Step)

### Step 1: Install Python

- Download **Python 3.10, 3.11, or 3.12** from: https://www.python.org/downloads/
- During installation, **check the box** that says **"Add Python to PATH"**
- Click Install

> ⚠️ **Do NOT use Python 3.13 or 3.14** — some packages may not support them yet.

### Step 2: Open Terminal in the Project Folder

- Open the `Tushar poject` folder in File Explorer
- Click on the address bar at the top and type `cmd` then press **Enter**
- A black terminal window will open pointing to this folder

### Step 3: Install Required Packages

Copy and paste this command into the terminal and press Enter:

```
pip install -r requirements.txt
```

This will install:
- **streamlit** — the web app framework
- **onnxruntime** — runs the AI model
- **pillow** — handles image processing
- **numpy** — numerical computations

### Step 4: Run the App

Copy and paste this command into the terminal and press Enter:

```
python -m streamlit run app.py
```

**OR** simply double-click the `run_app.bat` file.

### Step 5: Use the App

- Your default web browser will automatically open to `http://localhost:8501`
- Upload any **JPG or PNG** image of a cat or dog
- The AI will predict whether it's a Cat or a Dog with a confidence score
- Use the ☀️/🌙 button at the top to switch between Light and Dark mode

---

## 🔧 Troubleshooting

| Problem | Solution |
|---|---|
| `pip` is not recognized | Python is not added to PATH. Reinstall Python and check "Add to PATH" |
| `streamlit` is not recognized | Run: `python -m pip install streamlit` |
| Model files not found error | Make sure `mobilenetv2.onnx` and `imagenet_classes.txt` are in the same folder as `app.py` |
| Page is blank / won't load | Wait a few seconds, then refresh. First load takes time to load the model |
| Port 8501 is already in use | Close other Streamlit instances or run: `python -m streamlit run app.py --server.port 8502` |

---

## 📌 Quick Reference

```
# Install packages
pip install -r requirements.txt

# Run the app
python -m streamlit run app.py

# Run on a different port
python -m streamlit run app.py --server.port 8502
```

---

> 💡 **Tip:** Keep all the files together in the same folder. The app needs `mobilenetv2.onnx` and `imagenet_classes.txt` to be in the same directory as `app.py` to work.
