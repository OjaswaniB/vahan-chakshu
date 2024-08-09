# Real-Time IoT-Based Drowsiness Detection System

## Overview

This repository contains the code and documentation for a Real-Time IoT-Based Drowsiness Detection System, developed to enhance driver safety by detecting signs of drowsiness and alcohol consumption. The system utilizes an ensemble model combining VGG16, VGG19, and DenseNet to achieve high accuracy in identifying driver fatigue through facial expressions, head tilting, blinking, and yawning. Additionally, the system includes sensors for alcohol detection and post-crash analysis.

## Features

- **Drowsiness Detection**: Utilizes advanced deep learning models to monitor facial expressions, head tilting, blinking, and yawning to assess driver drowsiness.
- **High Accuracy**: Achieves 98% accuracy across various driving conditions.
- **Alert System**: Provides immediate alerts to the driver upon detecting fatigue and uses rotating motors to help the driver stay awake.
- **Alcohol Detection**: Integrated MQ3 sensor to detect alcohol levels in the driver’s breath.
- **Post-Crash Analysis**: Equipped with a gyroscope and accelerometer to analyze data following a collision.

## Components

1. **Ensemble Model**:
   - **VGG16**: A deep convolutional network model known for its simplicity and effectiveness in image classification tasks.
   - **VGG19**: An extension of VGG16 with additional layers, improving feature extraction capabilities.
   - **DenseNet**: A model that enhances performance by connecting each layer to every other layer in a feed-forward fashion.

2. **Sensors**:
   - **MQ3 Sensor**: Detects alcohol concentration in the breath.
   - **Gyroscope and Accelerometer**: Measures vehicle movements and orientation for post-crash analysis.

3. **Actuators**:
   - **Rotating Motors**: Activated to provide physical stimulation to the driver when drowsiness is detected.
