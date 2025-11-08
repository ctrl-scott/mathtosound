# Alphabet Roots Synth with Spectrogram 🎵

** ChatGPT Link**
[https://chatgpt.com/share/690e9e2b-646c-800c-bc70-aae6f9f9442c](https://chatgpt.com/share/690e9e2b-646c-800c-bc70-aae6f9f9442c)\
**Project:** `turning math to sound`

---

## 🧩 Overview

This project converts **letters (A–Z)** into **musical tones** using a mathematical mapping derived from **quadratic roots**.  
It blends **mathematics, sound synthesis, and visualization** — turning language into harmonic structures.

**Note** The roots were chosen by ChatGPT from the equations ChatGPT generated.

Every letter corresponds to a *root value* from a solved quadratic expression such as:

\[
x^2 + bx + c = 0
\]

These roots are used to offset a base pitch (A₄ = 440 Hz) by semitones, giving each letter a unique frequency.

The result:  
- Words → sequences of tones (melodies).  
- Names → harmonic chords.  
- Math → sound.

---

## 🎼 Core Equation

Each tone follows the cosine-wave relationship:

\[
y(t) = A \cos(2 \pi f t)
\]

Where:
- \( A \) = amplitude (0.6 by default)
- \( f \) = frequency in Hz
- \( t \) = time in seconds

---

## 🔢 Letter-to-Root Mapping

Each alphabet letter has an assigned quadratic root \( r(L) \):

| Letter | Root | Frequency (Hz) |
|:------:|:-----:|:---------------:|
| A | −2 | 392.00 |
| B | −1 | 415.30 |
| C |  2 | 493.88 |
| D | −2 | 392.00 |
| E |  1 | 466.16 |
| F | −4 | 370.00 |
| G | −5 | 349.23 |
| H | −4 | 370.00 |
| I | −5 | 349.23 |
| J |  4 | 554.37 |
| K | −4 | 370.00 |
| L | −2 | 392.00 |
| M |  3 | 523.25 |
| N | −3 | 370.00 |
| O |  1 | 466.16 |
| P | −5 | 349.23 |
| Q |  2 | 493.88 |
| R | −1 | 415.30 |
| S |  4 | 554.37 |
| T | −4 | 370.00 |
| U |  5 | 587.33 |
| V | −6 | 329.63 |
| W |  3 | 523.25 |
| X | −2 | 392.00 |
| Y |  1 | 466.16 |
| Z | −7 | 311.13 |

---

## 🎲 Mathematical Randomness

Each root came from factoring unique quadratic equations:

\[
x^2 + bx + c = 0
\]

For example:
- \( x^2 + 3x - 4 = (x + 4)(x - 1) \Rightarrow r = [-4, 1] \)
- \( x^2 - 9x + 20 = (x - 4)(x - 5) \Rightarrow r = [4, 5] \)

Only **one** root was chosen per letter — producing *structured randomness*:
- Different signs and magnitudes cause higher or lower pitches.
- The root distribution ensures both negative and positive offsets.
- This randomness gives the alphabet its musical variety.

---

## 💻 Features

- 🎧 **Real-time synthesis** using Web Audio API  
- 🌈 **Scrolling spectrogram** visualized via Canvas  
- ⌨️ **Type any word or phrase** → instantly converted to sound  
- 🎵 **Play as melody or chord** (letters sequentially or simultaneously)  
- 📊 **Dynamic letter–frequency table** auto-generated in the interface  
- 🧮 Based on real math: cosine waves, semitone offsets, and frequency ratios  

---

## 🧠 Conceptual Flow


Each layer adds mathematical structure while allowing creative randomness in tone generation.

---

## 🧰 Technical Implementation

**Core Technologies:**
- HTML5  
- JavaScript (Web Audio API + Canvas)  
- Inline CSS for compact educational deployment

**Key Components:**
- `AnalyserNode` → Real-time frequency capture  
- `Canvas` → Rolling spectrogram visualization  
- `OscillatorNode` → Generates sine (cosine-equivalent) tones  
- `GainNode` → Amplitude control  

---

## 🚀 Usage

1. Save the file as `alphabet_roots_synth_spectrogram.html`.
2. Open it in any modern browser (Chrome, Edge, Firefox).
3. Type any text (A–Z letters) in the input box.
4. Click **Play Melody** or **Play Chord**.
5. Watch the **spectrogram** light up with frequency bands that represent your text.

---

## 🧩 Example

**Input:**  

**Encoded roots:** [4, 2, 1, -4, -4]  
**Frequencies:** [554.37, 493.88, 466.16, 370.00, 370.00]  

Plays as both a five-tone sequence (melody) or harmonic stack (chord).

---

## 🧭 Educational Uses

- Demonstrate **waveforms, frequencies, and spectra** in an interactive way  
- Teach the link between **mathematics and sound synthesis**  
- Explore **chaotic order** from algebraic roots  
- Experiment with **cipher-music**, encoding words into tones  

---

## 📜 License

MIT License — for educational and non-commercial creative use.  
Attribution required if redistributed in modified form.

---

## 🧾 Citation

If referencing academically, cite as:

 (P.S. The format of theese citations need work if you try to use them)
> 2025. GitHub Repository. https://github.com/ctrl-scott/alphabet-roots-synth \
> Retrieved 2025. This YouTube Channel was also extremely helpful: [https://www.youtube.com/@brianmclogan](https://www.youtube.com/@brianmclogan)
---

## 🪶 Notes

This project continues the lineage of **mathematical sonification** —  
turning abstract logic into perceivable sound.  
Each letter’s randomness is deterministic, rooted in algebra —  
but collectively forms unique harmonic textures for every phrase.

---
