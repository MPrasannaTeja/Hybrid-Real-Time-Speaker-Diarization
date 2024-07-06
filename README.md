# Hybrid-Real-Time-Speaker-Diarization
A Hybrid Real-Time Speaker Diarization System that combines offline processing for accuracy with online subsystems for real-time performance
## Description
This project presents a novel Hybrid Real-Time Speaker Diarization System that combines offline processing for accuracy with online subsystems for real-time performance. Our approach leverages Mel-Frequency Cepstral Coefficients (MFCCs) for feature extraction, followed by low-rank deep embedding to obtain compact yet informative speaker representations.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)


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
```

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
## Contributing

Contributions are welcome! To contribute to this project, please follow these steps:

1. **Fork the Repository**: Click the "Fork" button at the top right of this repository's page.

2. **Clone Your Fork**: Clone your forked repository to your local machine.
    ```bash
    git clone https://github.com/your-username/Hybrid-Real-Time-Speaker-Diarization.git
    ```

3. **Create a Branch**: Create a new branch for your feature or bugfix.
    ```bash
    git checkout -b feature-name
    ```

4. **Make Changes**: Make your changes to the codebase.

5. **Commit Changes**: Commit your changes with a meaningful commit message.
    ```bash
    git add .
    git commit -m "Description of the changes you made"
    ```

6. **Push Changes**: Push your changes to your forked repository.
    ```bash
    git push origin feature-name
    ```

7. **Create a Pull Request**: Go to the original repository and create a pull request from your fork and branch. Describe your changes in detail and request a review.

8. **Review Process**: Participate in the review process. Make changes if required based on the feedback.

Please ensure that you follow the coding standards and write tests for your code. If you have any questions or need further assistance, feel free to open an issue to discuss your contribution.

Thank you for contributing!


