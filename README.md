# Teaching Algorithm Visualizer

Interactive teaching tool for BSD 404 (Algorithms II). Single-page web app built with HTML, CSS, JavaScript, and SVG.

## Overview

This project presents three algorithm modules in one unified interface with lecture notes, step-by-step simulation, pseudocode highlighting, operation counters, and interactive history playback.

1. Part 1: Floyd-Warshall (All-Pairs Shortest Paths)
2. Part 2: Fast Fourier Transform (FFT/DFT)
3. Part 3: Modular Exponentiation (Square-and-Multiply) + RSA

## Academic Context

- Course: BSD 404 - Algorithms II
- Instructor: Dr. Arash Kermani
- Student: Aggarwal, Parth
- Student ID: 20220001200

## Features

### Shared Platform Features

- Tab-based navigation across three parts
- Expandable lecture notes for each module
- Step/Play/Pause/Reset controls with adjustable playback speed
- Status badges, step counters, and jump-to-step history
- Responsive layout for desktop and mobile

### Part 1: Floyd-Warshall

- Preset graphs and custom matrix input
- Distance and predecessor matrix visualization
- Dynamic recurrence display and correctness invariant notes
- Guided prompts with prediction-and-reveal checkpoints
- Negative cycle detection and warning display
- Path reconstruction queries
- Complexity comparison panel

### Part 2: FFT / DFT

- Configurable signal generation (sine, square, chirp)
- Bit-reversal initialization and iterative butterfly stages
- Time-domain line chart and frequency-domain bar chart
- Twiddle factor and butterfly worked-step explanation
- Explicit problem statement, polynomial view, and O(N log N) derivation
- When-to-use guidance for FFT vs naive DFT
- Stage-wise operation counters and IFFT reconstruction check

### Part 3: Modular Exponentiation + RSA

- Left-to-right and right-to-left square-and-multiply variants
- Binary exponent bit-strip progression and worked trace
- RSA key generation, encryption, and decryption module
- Number theory notes: Euler's theorem, primality testing, CRT speedup
- RSA test vectors and factorization demo
- Operation counters for squaring and multiplication
- RSA preset for demonstration and BigInt verification

## Technical Design

- Single-file application architecture in index.html
- Vanilla JavaScript state machines per module
- Precomputed step arrays for deterministic playback
- SVG-based graph rendering and charting

## Project Structure

- index.html: Complete implementation (UI, styles, logic)
- project.md: Assignment requirements and project reference
- README.md: Project documentation

## Requirements

- Modern browser with JavaScript and SVG support
- BigInt support (for RSA) is required
- No build step or external dependencies

## Quick Start

1. Open index.html in any modern browser.
2. Use the top tabs to switch between Part 1, Part 2, and Part 3.
3. Expand lecture notes for conceptual context.
4. Click Build Steps and use playback controls to explore execution.

## Recommended Demo Flow

1. Start with Part 1 using the CLRS preset.
2. Build steps and show recurrence updates, then path reconstruction.
3. Switch to Part 2 and generate a signal with visible dominant bins.
4. Build FFT steps and explain one butterfly update.
5. Switch to Part 3 and run modular exponentiation with the RSA preset.
6. Show final verification and operation-count intuition.

## Notes

- RSA uses small demo keys and is not secure for real cryptography.
- FFT input size must be a power of two; the UI enforces this.
- Negative cycles make shortest paths undefined and are highlighted.
