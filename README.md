# MIDI Music Generation

Simple music generation with MIDI and neural networks.

Generate short melodies / note sequences using an LSTM (and optionally Magenta) trained on MIDI data.

**Part of a small music + ML series**:
- [spotify-music-recommender](https://github.com/S33mi/spotify-music-recommender) – content-based recommender + mood clusters
- [playlist-optimizer](https://github.com/S33mi/playlist-optimizer) – playlist creation as an optimization problem
- **This repo** – generative side (sequence modeling on MIDI)

---

## 🎯 Goal

Build a practical, end-to-end generative music pipeline:

1. Load and parse MIDI files
2. Convert notes into sequences suitable for a neural net
3. Train a small LSTM to predict the next note / chord
4. Generate new short melodies
5. Convert generated sequences back to MIDI and listen

Keep the scope focused and demoable (not a full Magenta research clone).

---

## 🔑 Key Features

- MIDI loading & preprocessing with `music21` / `pretty_midi`
- Note sequence encoding (pitch, duration, offset)
- LSTM (or simple Transformer later) for next-step prediction
- Temperature-controlled sampling for generation
- Export generated pieces to `.mid` files
- Optional: Magenta baseline for comparison

---

## 🛠️ Tech Stack

- **Python**
- **MIDI**: music21, pretty_midi
- **Deep Learning**: TensorFlow / Keras (or PyTorch)
- **Data**: numpy, pandas
- **Visualization**: matplotlib
- **Notebooks**: Jupyter / Colab

---

## 📁 Project Structure
