# Teaching Algorithm Visualizer

Professional interactive teaching tool for BSD 404 (Algorithms II), built as a single-page web application in HTML, CSS, JavaScript, and SVG.

## Overview

This project presents three algorithm modules in one unified interface with lecture notes, step-by-step simulation, pseudocode highlighting, operation counters, and interactive history playback.

1. Part 1: Floyd-Warshall (All-Pairs Shortest Paths)
2. Part 2: Fast Fourier Transform (FFT/DFT)
3. Part 3: Modular Exponentiation (Square-and-Multiply)

## Academic Context

- Course: BSD 404 — Algorithms II
- Instructor: Dr. Arash Kermani
- Student: Aggarwal, Parth
- Student ID: 20220001200

## Key Features

### Shared Platform Features

- Tab-based navigation across three parts
- Expandable lecture notes for each module
- Step, Play, Pause, Reset controls
- Adjustable playback speed
- Status badge and step counters
- History table with jump-to-step interaction
- Responsive layout for desktop and mobile

### Part 1: Floyd-Warshall

- Preset graphs and custom matrix input
- Distance matrix and predecessor matrix visualization
- Dynamic recurrence display for each transition
- Graph view with highlighted intermediate and active vertices
- Applied problem formulation and correctness invariant notes
- Guided prompts with prediction-and-reveal checkpoints
- Negative cycle detection and warning display
- Path reconstruction query between selected vertices
- Complexity comparison panel

### Part 2: FFT / DFT

- Configurable signal generation (sine, square, chirp)
- Bit-reversal initialization and iterative butterfly stages
- Time-domain line chart and frequency-domain bar chart
- Twiddle factor and butterfly worked-step explanation
- Explicit problem statement and FFT complexity derivation notes
- When-to-use guidance for FFT vs naive DFT
- Polynomial evaluation view (roots of unity)
- Stage-wise operation counters (butterflies, multiplications, additions)
- IFFT reconstruction quality check (max and average error)

### Part 3: Modular Exponentiation

- Left-to-right and right-to-left square-and-multiply variants
- Binary exponent bit-strip progression view
- Worked modular arithmetic trace per step
- Operation counters for squaring and multiplication
- RSA-style preset for demonstration
- Independent BigInt verification for result validation

## Technical Design

- Single-file application architecture in index.html
- Vanilla JavaScript state machines per module
- Precomputed step arrays for deterministic playback
- SVG-based graph rendering for Part 1
- Canvas-free chart rendering using SVG for Part 2
- Shared visual language and theme across all parts

## Project Structure

- index.html: Complete implementation (UI, styles, logic)
- project.md: Assignment requirements and project reference
- README.md: Professional project documentation

## How to Run

1. Open index.html in any modern browser.
2. Use the top tabs to switch between Part 1, Part 2, and Part 3.
3. Expand lecture notes for conceptual context.
4. Use Build Steps and playback controls to explore algorithm execution.

## Recommended Demo Flow

1. Start with Part 1 using CLRS preset.
2. Build steps and show recurrence updates, then path reconstruction.
3. Switch to Part 2 and generate a signal with visible dominant bins.
4. Build FFT steps and explain one butterfly update.
5. Switch to Part 3 and run modular exponentiation with RSA preset.
6. Show final verification and operation-count intuition.

## Quality Notes

- The interface emphasizes pedagogy: each visual step is paired with explanatory text.
- Algorithm traces are reproducible and reviewable through history navigation.
- The project is suitable for classroom demo, lab walkthrough, and report submission.
