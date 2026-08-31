# Hand Tracking Drawing App 🎨🤚

A real-time hand gesture based drawing application built with **MediaPipe** and **OpenCV**. Control everything with natural hand gestures - no mouse or keyboard needed for drawing!

![Demo](assets/demo.gif) <!-- Add a demo GIF if you have one -->

## ✨ Features

### 🖌️ **Natural Drawing**
- **Index finger only** → Draw smooth white lines
- Temporal smoothing (EMA) for jitter-free strokes
- Moving average stroke smoothing for clean lines

### 🤏 **Intuitive Object Manipulation (Pinch Gesture)**
- **Index + Middle finger tips together** → Grab objects
- **Move hand while pinched** → Translate selection
- **Spread fingers wider** → Scale UP
- **Bring fingers closer** → Scale DOWN
- **Rotate hand** → Rotate selection
- **Release pinch** → Drop object

### ✊ **View Control**
- **Fist (all fingers curled)** → Reset zoom/pan to default

### ⌨️ **Keyboard Shortcuts**
| Key | Action |
|-----|--------|
| `C` | Clear all drawings |
| `R` | Reset view (zoom/pan) |
| `Q` / `ESC` | Quit application |

### 🎯 **Visual Feedback**
- Real-time pinch distance display
- Selected object highlight (cyan bounding box)
- Pinch line visualization between fingertips
- Mode indicator (DRAW / PINCH_TRANSFORM / RESET / IDLE)
- Semi-transparent dark background for better visibility

## 🛠️ Tech Stack

- **Python 3.11+**
- **MediaPipe** (Hand Landmark Detection)
- **OpenCV** (Computer Vision & GUI)
- **NumPy** (Numerical computations)

## 🚀 Quick Start

### Prerequisites
```bash
pip install opencv-python mediapipe numpy
