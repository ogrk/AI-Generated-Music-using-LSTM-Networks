# 🎶 AI-Generated Music using LSTM Networks

### 🧠 NMIMS MPSTME | Department of Computer Science & Engineering  
**Submitted by:**  
- Devarsh Raval (E063)  
- Rishi Kaushik (E077)  
**Subject:** Artificial Intelligence  
**April 2025**

---

## 📖 Overview
This project explores the fusion of **Artificial Intelligence and music composition** using **Long Short-Term Memory (LSTM)** networks.  
The model learns musical patterns, chord progressions, and timing structures from **MIDI files**, and then generates entirely new compositions that reflect the learned style.  

A **Replit-based web interface** allows users to upload MIDI files, initiate model training, and download AI-generated compositions — no coding experience required.

---

## 🎯 Objectives
- Develop an AI model capable of learning musical structures from MIDI files using sequential modeling.  
- Generate original music compositions using an LSTM-based neural network.  
- Simplify user interaction with a web interface for uploading, training, and generating music.  
- Explore the creative potential of AI in music composition and human-AI collaboration.

---

## 🧩 Methodology

### 1. Data Collection
- MIDI files were sourced from open datasets across multiple genres and instruments to ensure musical diversity.

### 2. Data Preprocessing
- Used the **`music21`** library to parse and extract note sequences from MIDI files.  
- Encoded notes and chords as integers to feed into the model.

### 3. Model Training
- Implemented an **LSTM-based neural network** trained on note sequences.
- The model learns to predict the next note/chord in a musical sequence.

### 4. Music Generation
- After training, the model generates sequences of notes that are converted back to playable MIDI files.
- Adjustable parameters:
  - **Temperature:** Controls creativity/randomness of output.  
  - **Tempo:** Sets playback speed (BPM).  
  - **Sequence length:** Defines length of generated music.

### 5. Deployment
- Deployed using **Replit** with a minimal **Flask + HTML/CSS** interface.  
- Allows users to upload MIDI files, train small models, and download generated compositions directly from the browser.

---

## 🧱 Model Architecture

| Layer | Description |
|--------|--------------|
| **Input Layer** | Encodes sequences of notes |
| **Embedding Layer (optional)** | Converts tokens into dense vectors |
| **LSTM Layers** | Capture temporal dependencies in music |
| **Dropout Layer** | Prevents overfitting |
| **Dense Layer** | Predicts next possible note |
| **Activation** | Softmax for note probability distribution |

**Loss Function:** Categorical Cross-Entropy  
**Optimizer:** Adam  
**Framework:** TensorFlow / Keras  

---

## 💻 Implementation Details

**Language:** Python 3  
**Libraries Used:**  
- `tensorflow`, `keras`, `music21`, `numpy`, `pickle`, `random`, `flask`  
- **Frontend:** HTML/CSS (Replit Web App)

**Workflow:**
1. User uploads one or more MIDI files.  
2. The app extracts notes and preprocesses them.  
3. Model trains on the sequences.  
4. Generated MIDI output is made available for download.

---

## 🎧 Results and Outputs

### 🪄 Generated Music
- The model successfully generates **original MIDI compositions** that reflect musical styles from the training data.
- Outputs capture **chord progressions**, **melodies**, and **rhythmic structures** learned by the LSTM.

### 🎼 Style Adaptation
- Training on classical data → structured harmonic output.  
- Training on jazz/blues → improvised, swing-based sequences.  

### 🧠 Evaluation
- Subjective feedback showed the generated music was **coherent**, **pleasant**, and **stylistically similar** to the input datasets.  
- Evaluators found the results “surprisingly musical” and useful for further creative remixing.

---

## ⚙️ Challenges Faced
- MIDI file inconsistencies required robust preprocessing.  
- Limited training data caused occasional overfitting.  
- Replit’s compute constraints limited large-scale model training.  
- Capturing emotional depth and variety in music remains challenging.

---

## 🚀 Future Scope
- Integrate **Transformer** or **GPT-based** architectures for more complex compositions.  
- Enable **real-time music generation** or **VST plugin integration** for live performances.  
- Add **genre-based generation** and **emotion-conditioned outputs**.  
- Incorporate **human feedback loops** for iterative learning.  
- Expand into **collaborative AI-human composition tools**.

---

## 🌐 Web Interface (Replit)
The Replit app provides an intuitive, minimal interface that lets anyone:
- Upload MIDI files  
- Train an LSTM model  
- Generate new AI-composed tracks  
- Download and play the generated MIDI output  

👉 *This interface makes generative music accessible even to users without any programming background.*

---

## 🧩 Technologies Used
- **Python 3**
- **TensorFlow / Keras**
- **music21**
- **Flask (Replit Backend)**
- **HTML/CSS**
- **NumPy, Pickle, Random**

---

## 🧠 References
- Hochreiter & Schmidhuber (1997) — Long Short-Term Memory  
- [Google Magenta Project](https://magenta.tensorflow.org/)  
- [OpenAI MuseNet](https://openai.com/research/musenet)  
- [Music21 Documentation](http://web.mit.edu/music21/)  
- [A.I. Duet by Google](https://experiments.withgoogle.com/ai/ai-duet/view/)

---

## 👥 Contributors

- **Rishi Kaushik [@ogrk](https://github.com/ogrk)** 
- **Devarsh Raval [@Devarsh-Raval](https://github.com/Devarsh-Raval)**   

---

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
