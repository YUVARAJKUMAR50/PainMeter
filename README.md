# PainMeter
Pain assessment and management remain major challenges in healthcare, as conventional tools such as the Visual Analog Scale and Numerical Rating Scale depend entirely on patient self reporting. These subjective methods are often unreliable, especially for patients who are unconscious, non verbal, or unable to communicate effectively. To address this gap, this project proposes a dual-function device capable of both pain detection and Tens Machine for pain relief.
# Project Description
This project presents a multisensor-based embedded system to estimate pain-related physiological responses and provide assistive pain relief therapy. The system integrates temperature, heart rate, and EMG sensors to observe physiological patterns associated with pain and stress. An ESP32 microcontroller collects and processes the sensor data and infers a probable pain condition using combined sensor analysis. The system does not directly measure pain but estimates it based on physiological indicators. Based on the inferred condition, a commercially certified TENS therapy module is activated for assistive pain relief. Local visualization is provided using an LCD/OLED display, with optional IoT support for remote monitoring.
# System Overview
The system consists of two integrated modules: Pain Detection and Ultrasonic Therapy. The ESP32 microcontroller serves as the central hub, collecting data, analyzing signals, and triggering therapy while simultaneously uploading results to Blynk Cloud.
## Pain Detection Sensors
GSR Sensor – Measures changes in skin resistance; higher conductance indicates sympathetic activation during pain.
EMG Sensor – Captures electrical muscle signals; abnormal spikes indicate pain-related muscle activity.
MAX30102 – Provides heart rate and oxygen saturation, both of which change during pain.
EMG (Electromyography) sensor – Measures muscle activation by sensing electrical signals generated during muscle contraction.
## AI/ML Module
A camera module captures the subject’s facial expressions.
Pre-trained CNN models detect pain-related expressions (eyebrow contraction, eye squeeze, mouth grimacing).
ML integration ensures the system adapts to individual pain tolerance, reducing false positives.
## Therapy Module
A TENS (Transcutaneous Electrical Nerve Stimulation) module is used to deliver low-voltage electrical pulses.
Activated automatically upon confirmed pain detection or manually via a control button.
Provides safe, non-invasive, drug-free pain relief by modulating nerve signals and reducing pain perception.
## IoT Integration
Blynk Cloud stores and visualizes sensor readings in real time.
Clinicians can monitor pain events, heart rate trends, and therapy sessions remotely through a smartphone app.

