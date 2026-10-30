# S-HPFL – Privacy-Preserving Hierarchical Personalized Federated Learning for Online Exam Proctoring

## Project Overview

S-HPFL is an AI-powered online examination proctoring system designed to improve examination security through intelligent monitoring and privacy-preserving machine learning.

The system integrates Artificial Intelligence (AI), Computer Vision, Deep Learning, and Hierarchical Personalized Federated Learning to detect suspicious activities during online examinations while supporting privacy-aware collaborative model training.

Unlike traditional online proctoring systems that rely on centralized data collection, S-HPFL incorporates Federated Learning techniques to support local model training and collaborative model aggregation without exporting raw proctoring data.

## Key Features

- **AI-Based Proctoring:** Monitors examination activities using computer vision and audio analysis.
- **Face Detection and Recognition:** Detects faces and verifies student identity.
- **Object Detection:** Identifies potentially prohibited objects such as mobile phones, laptops, and books.
- **Head and Hand Gesture Detection:** Monitors suspicious head movements and hand gestures.
- **Audio Monitoring:** Detects suspicious talking and sound activities.
- **Risk Assessment:** Assigns risk scores based on detected suspicious activities.
- **Automated Warnings:** Generates warnings based on risk levels.
- **Federated Learning:** Supports collaborative model training without sharing raw training data.
- **FedAvg and FedProx:** Implements federated optimization and aggregation techniques.
- **Differential Privacy:** Applies gradient clipping and noise addition during local training.
- **Hierarchical Aggregation:** Supports student-level, institution-level, and global-level model aggregation.
- **Personalized Federated Learning:** Supports local model personalization for individual clients.

## Technologies Used

**Frontend**
- React.js
- Vite
- JavaScript
- CSS

**Backend**
- Python
- FastAPI
- REST APIs

**Artificial Intelligence and Machine Learning**
- PyTorch
- Computer Vision
- Deep Learning
- Face Recognition
- Object Detection
- Audio Classification

**Federated Learning**
- Federated Averaging (FedAvg)
- Federated Proximal (FedProx)
- Hierarchical Federated Learning
- Personalized Federated Learning
- Differential Privacy
- DP-SGD

**Desktop Application**
- Electron.js

**Database and Tools**
- SQL Database
- Git and GitHub
- Swagger UI

## Federated Learning Architecture

The proposed S-HPFL architecture consists of three logical levels:

1. **Student-Level Training:** Each client performs local model training using its available proctoring features.
2. **Institution-Level Aggregation:** Institution-level servers aggregate client model updates using FedAvg.
3. **Global-Level Aggregation:** The global server aggregates institution-level model parameters to update the global model.

Personalized learning allows individual clients to further adapt the shared model to their local data.

## Privacy Protection

S-HPFL incorporates Differential Privacy using DP-SGD techniques, including gradient clipping and Gaussian noise addition.

The federated learning workflow is designed to exchange model parameters rather than raw examination media or biometric data.

## Current Implementation Status

- React frontend and FastAPI backend implemented.
- Electron-based secure examination client implemented.
- AI-based proctoring and risk assessment integrated.
- Local personalized FL training tested.
- Institution-level FedAvg API tested.
- Global-level FedAvg API tested.
- Differential Privacy training tested.
- Controlled multi-client research experiments conducted using synthetic datasets.

**Note:** The live API aggregation tests currently demonstrate one client and one institution. Deployment on separate physical client machines and cloud infrastructure remains future work.

## Project Objective

The primary objective of S-HPFL is to develop a secure, intelligent, and privacy-aware online examination proctoring framework by combining AI-based suspicious activity detection with hierarchical personalized federated learning.

## Future Enhancements

- Multi-client federated learning validation across independent devices.
- Cloud-based deployment.
- Improved model performance using real-world proctoring datasets.
- Persistent federated model storage and synchronization.
- Scalability and performance evaluation.

## Project Type

Academic Project – AI, Machine Learning, and Federated Learning.
