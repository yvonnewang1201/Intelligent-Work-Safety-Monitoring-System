# Intelligent-Work-Safety-Monitoring-System
ntelligent Work Safety Monitoring System - Server Dashboard
This repository contains the server-side implementation of an IoT-based industrial safety monitoring system. The system is designed to aggregate real-time video streams from multiple edge devices (clients) performing MediaPipe-based posture analysis.

Core Features
Multi-Client Handling: Utilizes Python's threading library to manage concurrent TCP connections from various factory workstations.

Real-Time Data Streaming: Implements custom socket communication protocols with struct and pickle for efficient image serialization and transmission.

Dynamic UI Dashboard: A built-in GUI developed with Tkinter that dynamically adjusts a grid layout to display up to 5 concurrent worker safety feeds.

Live Frame Processing: Integrates OpenCV (cv2) for on-the-fly image decoding and rendering onto a high-performance Canvas widget.

Technical Stack
Networking: Socket Programming (TCP/IP), Struct, Pickle.

Concurrency: Multi-threading.

Computer Vision: OpenCV (cv2).

GUI: Tkinter, PIL (Pillow).

Language: Python 3.x.

How It Works
The server acts as a central hub in an industrial environment. Each "worker station" (client) captures video, processes skeletal landmarks via MediaPipe, and streams the processed frames to this server. The server then visualizes these risks in a centralized dashboard for safety supervisors.

Conference Publication
This project was part of the research presented at the TANET 2024 Conference, focusing on innovative and practical applications of IoT and Computer Vision in workplace safety.
