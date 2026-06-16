# hand-gesture-particle-explode
# Wonderstone Particle Matrix (Explode)

An advanced, interactive WebGL physics simulation that maps 20,000 dynamic particle entities directly to real-time physical hand coordinates and gestures using your webcam.


[Live Interactive Demo Link]
https://sathvikachandramohan.github.io/hand-gesture-particle-explode/

---

## Project Description
**Wonderstone Particle Matrix** is a computer vision and frontend graphics experiment that brings kinetic control environments to the browser. By combining high-performance particle buffers in WebGL with lightweight machine learning hand tracking models, the application processes real-time video frames to map coordinates, toggle physics states, and apply acceleration forces across thousands of mathematical particles seamlessly.

---

## Overview
This project was built to experiment with zero-latency computer vision interactions directly on the client side. By calculating fluid mechanics, drag vectors, and distance thresholds between floating coordinates and MediaPipe hand tracking arrays, it translates computer vision data directly into structural motion without requiring complex desktop software setups.

---

## Project Objectives
- **Computer Vision Normalization:** Successfully map 2D camera viewport landmark tracking matrices onto responsive 3D WebGL perspective fields.
- **High-Performance Rendering:** Manipulate structural `Float32Array` positional buffers inside raw geometry instances to render 20,000 particles smoothly at 60 FPS.
- **Gesture State Mapping:** Implement complex mathematical rule checks (distance vector thresholds) to translate skeletal finger movements into interactive physics engines.

---

## Implemented Features

###  Visuals & High-Performance WebGL
- **20,000 Vertex Systems:** Uses a customized `THREE.BufferGeometry` pipeline optimized for processing coordinates with hardware acceleration.
- **Additive Canvas Blending:** Utilizes custom blend modes (`THREE.AdditiveBlending`) alongside transparency rules to make thousands of microscopic coordinates glow with intense luminosity.
- **Responsive Display Deck:** Adapts dynamically to window resizing constraints, reconstructing projection aspect ratios on the fly.

###  Gesture Rules & Dynamic Physics States
As you look at your webcam, the custom JavaScript logic calculates multi-point distances to toggle between three interaction profiles:
-  **Attract & Swirl (Default Open Palm):** Particles track your index finger coordinate profile. If they get closer than 22 units, a tangential vector force pulls them into an organic spinning cosmic vortex.
- **Fist (Charging Explosion):** Measures the average geometric distance from all finger tips to your wrist landmark. When a closed fist is formed, it pulls all 20,000 particles tightly into a high-density trembling core point.
- **Shockwave Release:** Opening your hand immediately following a fist trigger sets off an explosive outward force vector that repels nearby particles inversely proportional to their distance from your palm.
- **Pinch (Cycle Color Presets):** Checks the absolute distance between your thumb tip and index finger. Pinching cleanly shifts the matrix between 3 unique color profiles: **Cosmic** (Deep blues/purples), **Fire** (Intense reds/oranges), and **Emerald** (Vivid greens).

---

## Technologies Used
- **Three.js (r128):** Hardware-accelerated WebGL engine for rendering vector structures, buffer attributes, and additive glowing points.
- **MediaPipe Hands:** Google's machine learning tracking framework to capture 21 distinct skeletal hand nodes from incoming video arrays.
- **MediaPipe Camera Utils:** Helper extensions to capture low-overhead webcam image frame buffers.
- **HTML5 & CSS3:** Full-screen responsive tracking canvas wrapper combined with absolute overlay heads-up displays (HUD).

---

## Project Structure
```text
wonderstone-particle-matrix/
│
└── index.html   # Standalone bundle containing UI overlays, WebGL setups, tracking math, and physics pipelines
