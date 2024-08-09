# Real-Time IoT-Based Drowsiness Detection System - VAHAN CHAKSHU
This Real-Time IoT-Based Drowsiness Detection System leverages the machine learning life cycle to ensure accurate and effective detection of drowsiness. The machine learning life cycle includes several key stages, each of which is crucial for developing a robust system. Below is an overview of how each stage is applied in our system:

![image](https://github.com/user-attachments/assets/03e974dc-752f-4af8-a6c7-02d48aee3654)

## Objective
The system utilizes an ensemble model combining VGG16, VGG19, and DenseNet to achieve high accuracy in identifying driver fatigue through facial expressions, head tilting, blinking, and yawning. Additionally, the system includes sensors for alcohol detection and post-crash analysis.


## Data Preparation
Due to lack of existing dataset, we created a dataset of **14,500** images. The methodologies followed were-
- **Video Recording**: Cameras were set up to record drivers' facial expressions, specifically
focusing on eye movements and head positions. This allowed for detailed analysis of
blinking patterns and head nodding.
- **Manual Observation**: We manually observed and recorded instances of different
states during driving simulations or real-world scenarios. 

## Classes
- **Neutral**: The driver is in a normal, alert state. Eye blink rates and head nods are within
typical ranges for a person who is fully awake and attentive.

![image](https://github.com/user-attachments/assets/0d73d231-c7a1-4bb8-a85b-82443452002f)

- **Yawning**: This category indicates a higher likelihood of drowsiness. Yawning is often a
visible sign of fatigue, and the dataset may include instances where the driver yawns or
shows signs of being tired.

![image](https://github.com/user-attachments/assets/8cb47a47-afb8-44ee-8f8d-f3d51e3a509f)

- **Eyes Closed**: This state is characterized by the driver having their eyes fully closed. It
could signify extreme drowsiness or inattentiveness, and the data collection would record
how long and frequently this occurs.

![image](https://github.com/user-attachments/assets/9a00299d-70c7-4003-ba80-87364714513a)

- **Drowsy**: The driver exhibits signs of drowsiness beyond just yawning or closed eyes. This
might include slow and frequent blinking, prolonged eye closure, or nodding off.

![image](https://github.com/user-attachments/assets/485056d6-2a87-414e-bb92-cdefd9b60e62)

- **Half Open Eyes**: This state shows a transition between being awake and
falling asleep. It represents a condition where the driver’s eyes are not fully open but are
not fully closed either, indicating varying levels of alertness.

![image](https://github.com/user-attachments/assets/de1b35da-d694-450f-9220-ee01df84a662)

## Model Building
Trained machine learning models using labeled datasets that included various levels of driver drowsiness. Models included VGG16, VGG19 and DenseNet that were amalgamated using voting method in ensembling. 


## Features

- **Drowsiness Detection**: Utilizes advanced deep learning models to monitor facial expressions, head tilting, blinking, and yawning to assess driver drowsiness.
- **Alert System**: Provides immediate alerts to the driver upon detecting fatigue and uses rotating motors to help the driver stay awake.
- **Alcohol Detection**: Integrated MQ3 sensor to detect alcohol levels in the driver’s breath.
- **Post-Crash Analysis**: Equipped with a gyroscope and accelerometer to analyze data following a collision.

## Deployment Components

1. **Ensemble Model**:
   - **VGG16**: A deep convolutional network model known for its simplicity and effectiveness in image classification tasks.
   - **VGG19**: An extension of VGG16 with additional layers, improving feature extraction capabilities.
   - **DenseNet**: A model that enhances performance by connecting each layer to every other layer in a feed-forward fashion.

2. **Sensors**:
   - **MQ3 Sensor**: Detects alcohol concentration in the breath.
   - **Gyroscope and Accelerometer**: Measures vehicle movements and orientation for post-crash analysis.

3. **Actuators**:
   - **Rotating Motors**: Activated to provide physical stimulation to the driver when drowsiness is detected.
  
## Monitoring
The system achieved an accuracy rate of 85%, 82% and 90% in VGG16, VGG19 & DenseNet respectively in detecting drowsiness, based on test data from controlled environments.

![image](https://github.com/user-attachments/assets/d7f2121d-541f-42e7-8451-1aea82439ff5)


## References
Driver drowsiness detection and smart alerting using deep learning and IoT Anh-Cang Phan a,∗, Thanh-Ngoan Trieu b,c, Thuong-Cang Phan c a Vinh Long University of Technology Education, Vinh Long, 85110, Viet Nam b Université de Bretagne Occidentale, Brest, 29200, France c Can Tho University, Can Tho, 94115, Viet Nam

