# 🛸 G-BOARD | Spatial Vision Keyboard OS (V6.0)

> **A High-Performance WebGL & Computer Vision Spatial Input Interface Built with MediaPipe, Web Audio API, and Modern JavaScript.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![MediaPipe Tasks](https://img.shields.io/badge/Vision-MediaPipe%20Hands-00f2ff.svg)](https://developers.google.com/mediapipe)
[![Deployment: Vercel](https://img.shields.io/badge/Deployment-Vercel%20HTTPS-black.svg)](https://vercel.com)
[![WCAG Standard](https://img.shields.io/badge/Accessibility-WCAG%202.1%20Compliant-brightgreen.svg)](https://www.w3.org/WAI/standards-guidelines/wcag/)



## 📌 Executive Summary

**G-BOARD (Ghost Keyboard)** is an accessible, touchless spatial keyboard application operating natively in the browser via standard webcams. Utilizing real-time 3D skeletal hand tracking, spatial coordinate mapping, and dynamic dwell-state execution, G-BOARD provides a contactless typing environment with live environmental telemetry, synthesized speech output, and haptic feedback profiles.



## 🚀 Key System Features

* **Multi-Hand Skeletal Tracking:** Real-time tracking of 21 3D hand landmarks powered by MediaPipe.
* **Spatial Fingertip Reticle:** Dynamic cursor following the index fingertip (Landmark 8) for immediate visual confirmation.
* **Dual-Stage Clear Logic:**
  * `0.75s` Dwell: Single Character Backspace.
  * `1.50s` Dwell: Buffer Flush.
* **Haptic Audio & Visual Synthesis:** Real-time Web Audio API frequency ramps paired with glassmorphism hover transitions.
* **Voice Readout Engine:** Web Speech API integration (`SPEAK` Key) for instant output vocalization.
* **Live Environmental Telemetry HUD:**
  * High-Accuracy Geolocation & Reverse Geocoding via BigDataCloud API.
  * Live satellite weather via Open-Meteo REST API.
  * Words Per Minute (WPM) engine and live character counter.
* **Cyberpunk Visual Profiles:** Toggleable UI profiles (Stark Cyan, Amber, Crimson) using CSS Custom Properties.



## 🛠 Tech Stack & Architecture

| Layer | Technologies Used |
| :--- | :--- |
| **Computer Vision Core** | MediaPipe Hands API, HTML5 Canvas, WebGL |
| **Frontend HUD Interface** | HTML5, CSS3 Glassmorphism, Google Fonts (`Orbitron`) |
| **Haptics & Audio** | Web Audio API (`OscillatorNode` & `GainNode`) |
| **Speech Engine** | Web Speech API (`SpeechSynthesisUtterance`) |
| **Telemetry Services** | HTML5 Geolocation API, Open-Meteo REST API, BigDataCloud |