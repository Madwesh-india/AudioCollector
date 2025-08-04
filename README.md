# 🎙️ Bilingual Audio Recorder (English & Tulu)

An interactive Python tool to record bilingual speech samples using **PyAudio** and **ipywidgets** in a Jupyter Notebook. Ideal for collecting aligned audio datasets (e.g., English ↔ Tulu) for speech recognition, language translation, or linguistic research.

---

## 📦 Features

- ✅ Record audio for two separate languages (English and Tulu)
- 🧠 Interactive UI using `ipywidgets` for Start/Stop per language
- 💾 Automatically stores WAV files with a unique random ID
- 📝 Input label field and CSV logging (`data.csv`)
- ❌ Cancel button to discard unwanted recordings
- 📂 Organizes files into separate folders (`ENGLISH/`, `TULU/`)

---

## 🛠️ Requirements

- Python 3.7+
- `pyaudio`
- `ipywidgets`
- Jupyter Notebook or JupyterLab

### Install dependencies

```bash
pip install pyaudio ipywidgets
````

For Linux, if PyAudio fails to install:

```bash
sudo apt-get install portaudio19-dev
pip install pyaudio
```

---

## 🚀 How to Use

1. Launch your Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
2. Open the notebook containing the code.
3. Click **Start Recording ENGLISH** and **Start Recording TULU** as needed.
4. Click **Stop** when done.
5. Enter the associated label/text in the input box.
6. Press **NEXT** to save the label in `data.csv`.
7. If you want to discard the current recording pair, press **Cancel**.

Files will be saved as:

```
ENGLISH/<randomID>.wav
TULU/<randomID>.wav
```

And your CSV (`data.csv`) will contain:

```
<randomID>,<user_input_text>
```

---

## 🧩 Project Structure

```
bilingual-audio-recorder/
├── ENGLISH/               # Saved English audio files
├── TULU/                  # Saved Tulu audio files
├── data.csv               # Text labels for each recording pair
├── notebook.ipynb         # Main notebook (contains all UI and logic)
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! If you'd like to:

* Add support for more languages
* Include audio visualizations
* Improve file organization
  Feel free to open an issue or submit a pull request.

---

## 📜 License

MIT License
