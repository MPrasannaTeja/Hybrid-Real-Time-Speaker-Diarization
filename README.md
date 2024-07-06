# Hybrid-Real-Time-Speaker-Diarization
A Hybrid Real-Time Speaker Diarization System that combines offline processing for accuracy with online subsystems for real-time performance
## Description
This project presents a novel Hybrid Real-Time Speaker Diarization System that combines offline processing for accuracy with online subsystems for real-time performance. Our approach leverages Mel-Frequency Cepstral Coefficients (MFCCs) for feature extraction, followed by low-rank deep embedding to obtain compact yet informative speaker representations.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Speaker diarization is the process of segmenting and labeling audio data based on speaker identities. This project aims to develop a hybrid system that integrates both offline and online subsystems to achieve continuous and accurate speaker diarization.

## Features
- **Offline Processing**: High accuracy through comprehensive analysis of accumulated data.
- **Online Processing**: Real-time adaptation and speaker labeling with minimal latency.
- **Hybrid Architecture**: Combines the strengths of both offline and online subsystems.

## Installation
To install the necessary dependencies, run the following command:
```bash
pip install -r requirements.txt

## Usage

1. **Feature Extraction**:
    ```python
    from src import feature_extraction
    mfcc_features = feature_extraction.extract_mfcc(audio_file)
    ```

2. **Offline Processing**:
    ```python
    from src import offline_processing
    speaker_segments = offline_processing.process_audio(mfcc_features)
    ```

3. **Online Processing**:
    ```python
    from src import online_processing
    real_time_labels = online_processing.process_stream(audio_stream)
    ```

4. **Hybrid System**:
    ```python
    from src import hybrid_system
    hybrid_labels = hybrid_system.process(audio_file)
    ```

