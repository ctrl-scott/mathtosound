# Alphabet Roots Synth with Spectrogram 🎵


**Project:** `turning math to sound`

---

## 🧩 Overview

This project converts **letters (A–Z)** into **musical tones** using a mathematical mapping derived from **quadratic roots**.  
It blends **mathematics, sound synthesis, and visualization** — turning language into harmonic structures.

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

