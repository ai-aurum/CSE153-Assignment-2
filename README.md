# CSE 153 Assignment 2 - Symbolic Music Generation

## Project Overview
This assignment implements two tasks in symbolic music generation using ML techniques: <br>
1. **Symbolic Unconditional Generation:** 
   Used a first order Markov Chain.
2. **Symbolic Conditional Generation:**
   Used an LSTM based Recurrent Neural Network (RNN).
   
The music is generated from MIDI data, specifically using the [MAESTRO v3.0.0 dataset](https://magenta.tensorflow.org/datasets/maestro).

### Video Presentaion
Linked separately via [Google Drive]().

## Setup and Dependencies
The following Python packages must be installed to properly execute the notebook:
```
pip install torch torchvision torch audio
pip install numpy miditok symusic miditoolkit midi2audio
```
Additionally, FluidSynth must be installed on your system:
- MacOS:
  ```
  brew install fluid-synth
  ```
- Ubuntu/Linux:
  ```
  sudo apt-get install fluidsynth
  ```
Verify its installation with:
```
fluidsynth --version
```

## Files Provided
- `symbolic_unconditioned.mid`: MIDI file generated using the Markov Chain model.
- `symbolic_unconditioned.wav`: Audio file converted from the generate MIDI.
- `symbolic_conditioned.mid`: MIDI file generated using the LSTM based hormonization model.
- `rnn.mid`: Additional MIDI file generate using the LSTM based harmonization model.
- `rnn.wav`: Audio file converted from the additional generate MIDI.
- `workbook.ipynb`: Jupyter notebook with each step of data processing, modeling, training, and evaluation for both tasks.
- `README.md`: This documentation file.

## How to Run:
1. Ensure setup and dependencies are all installed.
2. Open the provided Jupyter notebook *workbook.ipynb**
3. To regenerate MIDI and audio files execute the notebook cells to train models and generate music.

The generated files (.mid and .wav) can be directly opened with standard media players.

