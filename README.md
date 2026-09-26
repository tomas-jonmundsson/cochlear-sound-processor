# Cochlear Implant Sound Processing — Electrodogram GUI

**Biomedical Engineering | University of Sydney | 2026**

Python implementation of three clinical cochlear implant sound processing strategies — F0F1F2, ACE, and CIS — producing a Frequency-Time Matrix for vocoder playback and generating a real-time electrodogram from audio input.

## Overview

Cochlear implants encode sound through electrical stimulation of the auditory nerve via an electrode array. This project implements the signal processing pipeline behind three standard stimulation strategies, with a full GUI for clinical and educational exploration.

## Sound Processing Strategies

| Strategy | Description |
|---|---|
| **F0F1F2** | Extracts fundamental frequency and first two formants |
| **ACE** | Advanced Combinational Encoder — selects n highest-energy channels per cycle |
| **CIS** | Continuous Interleaved Sampling — stimulates all channels in rapid sequence |

## Features

- `.WAV` file input or live microphone capture
- Real-time time-domain signal visualisation
- Electrodogram output display (Frequency-Time Matrix)
- Vocoder playback of encoded signal
- Strategy selection via radio buttons (F0F1F2 / ACE / CIS)
- RUN, PLAY RESULT, PLAY WAV controls

## GUI

Built in Python with an intuitive interface designed for clinical usability — no command-line interaction required.

## Tech Stack

`Python` `NumPy` `SciPy` `Matplotlib` / `Tkinter` `Audio Signal Processing`

## Files

- `main.py` — Application entry point and GUI
- `processing/f0f1f2.py` — F0F1F2 strategy implementation
- `processing/ace.py` — ACE strategy implementation
- `processing/cis.py` — CIS strategy implementation
- `vocoder/` — Vocoder playback engine
- `report.pdf` — Full project report

## Key Takeaways

- Implements three clinically-used cochlear implant processing standards from first principles
- Full-stack deliverable: audio signal processing pipeline integrated with a functional GUI
- Designed for accessibility — usable by clinicians or researchers without programming knowledge
