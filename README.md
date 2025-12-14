        AI-Based Future Fabrication System Using Physiological and Visual Parameters

 Abstract
This project presents an AI-driven fabrication system that integrates physiological
signals and visual parameters to dynamically recommend fabrication strategies.

   Technologies Used
- Python
- TensorFlow (CNN)
- OpenCV
- Arduino
- Machine Learning

#Project Structure

AI_Fabrication_System_DL/
│
├── arduino_sensor.ino
├── cnn_model.py
├── visual_module.py
├── physiological_module.py
├── decision_engine.py
├── fabrication_output.py
├── main.py
├── paper/
│   └── Journal_Paper.pdf
├── figures/
│   └── architecture.png
└── README.md
arduino_sensor.ino

This file contains the Arduino program responsible for collecting physiological parameters such as heart rate, skin temperature, and stress level. The sensor data is transmitted to the Python application through serial communication, representing the hardware sensing layer of the system.

cnn_model.py

This module defines the Convolutional Neural Network (CNN) using TensorFlow. It performs deep learning–based feature extraction and classification from visual input data, forming the core artificial intelligence component of the project.

visual_module.py

This file handles visual data acquisition using a webcam. It captures images, preprocesses them (grayscale conversion, resizing, normalization), and prepares the input data for the CNN model.

physiological_module.py
This module reads physiological sensor values sent by the Arduino via serial communication. It converts the received data into numerical arrays suitable for AI-based decision-making.

decision_engine.py

This file integrates outputs from the CNN model and physiological data analysis. It acts as the decision-making unit that determines the appropriate fabrication strategy based on combined human parameters.

fabrication_output.py

This module translates AI decisions into fabrication recommendations such as soft wearable materials, rigid support structures, or adaptive smart fabrics, simulating an automated future fabrication system.

main.py

This is the main execution file that controls the overall workflow. It coordinates visual input acquisition, physiological data reading, AI-based decision processing, and fabrication output generation.

paper/Journal_Paper.pdf

This folder contains the research journal paper associated with the project. It documents the problemstatement, methodology, system architecture, results, and future scope of the work.

figures/architecture.png

This directory stores visual assets such as system architecture diagrams and flowcharts used in the journal paper and project documentation.

README.md

This file provides a comprehensive overview of the project, including objectives, system description, installation steps, execution instructions, technologies used, and references to the journal paper.

