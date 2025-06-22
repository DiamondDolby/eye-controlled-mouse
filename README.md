
# Eye-Controlled Mouse with Blink Click Detection

This project uses **MediaPipe**, **OpenCV**, and **PyAutoGUI** to create a real-time system that moves the mouse cursor based on eye movement and triggers a click using blink detection. It's a lightweight hands-free interface that can be used for accessibility, automation, or experiments in human-computer interaction.

## 🚀 Features

- 🖱️ Move your mouse cursor using your eye movement.
- 👁️ Blink (left eye) to click — no hands needed.
- Real-time feedback with camera preview and blink threshold debugging.

## 🧰 Technologies Used

- Python 3.7+
- [MediaPipe](https://google.github.io/mediapipe/)
- OpenCV
- PyAutoGUI

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/eye-mouse-controller.git
   cd eye-mouse-controller
   ```

2. **Install dependencies**
   ```bash
   pip install opencv-python mediapipe pyautogui
   ```

> ⚠️ PyAutoGUI controls your actual mouse — be careful during testing.

## ▶️ How to Run

```bash
python mainV1.0.py
```

1. A webcam window will appear.
2. Look around — your eyes will move the cursor.
3. Blink your **left eye** to simulate a mouse click.
4. Press `Ctrl+C` or close the camera window to stop.

## 🛠️ Adjustments

- **Blink threshold** is set to `0.015`. If clicks trigger too often or not enough, adjust the value in the code:
  ```python
  if diff < 0.015:
  ```

- **Click delay** is hardcoded to 1 second (`time.sleep(1)`) to avoid multiple triggers — tune this if needed.

## 📷 Demo

> Add demo video or GIF here if available.

## 🤖 Future Improvements

- Calibration step to auto-detect blink threshold.
- Multi-eye detection for left/right blink actions.
- Drag-and-drop or scrolling based on facial gestures.

## 🙋‍♂️ Author

Sharavanan Mathivanan  
Feel free to connect or reach out for collaboration.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
