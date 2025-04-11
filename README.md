# 🚦 Traffic Sign recognition on ESP32-CAM with CNN & Audio Feedback

A low-cost, real-time traffic sign recognition system for Intelligent Transportation Systems (ITS), using ESP32-CAM and a custom-trained CNN model with audio announcements for accessibility.

Overview
This project captures live traffic sign images using an ESP32-CAM, classifies them using a TensorFlow Lite CNN model, and provides audio feedback via an MP3-TF-16P module — aiding both driver assistance and visually impaired users.

-  **Accuracy**: 94.00% on GTSRB test data  
- **Audio Feedback**: Pre-recorded voice for recognized signs  
- **Edge Deployment**: Optimized for memory-limited devices  

##  Hardware Components
- **ESP32-CAM** – image capture & processing  
- **MP3-TF-16P** – plays sign names through speaker  
- **MicroSD Card** – stores model & audio files  

##  Model Summary
- **Input**: 64×64 RGB images  
- **Output**: 42 traffic sign classes  
- **Architecture**: 3 Conv layers → MaxPooling → Dropout → Dense → Softmax  
- **Trained With**: TensorFlow/Keras → Converted to TFLite  
 
