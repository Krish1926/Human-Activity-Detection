# Human-Activity-Detection
Introduction 
Context: Human Activity Recognition (HAR) is vital for healthcare, eldercare, and wearable tech.
Problem: Traditional systems struggle with accuracy and computational efficiency.
Solution: Ensemble learning with meta-classifiers to improve robustness and performance.
Aim: Design an optimized framework for accurate and efficient HAR using sensor data.

# Data Set and Preprocessing
HARSense Dataset:
Sensors: Accelerometer, Gyroscope, Magnetometer.
Features: Mean, Std, Min, Max, RMS (x, y, z axes).
Activities: Walking (10,052), Sitting (12,766), Running (9,620), etc.
Preprocessing Steps:
Removed 44,624 duplicates (final: 49,574 rows).
Downsampled to balance classes.
Encoded categorical labels (LabelEncoder).
Normalized features (StandardScaler).
80-20 train-test split (21,509 train, 5,378 perspective

