
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
   git clone https://github.com/DiamondDolby/vision-mouse.git
   cd vision-mouse
   ```

2. **Install dependencies**
   #### Option A: if you have requirements.txt
   ```bash
   pip install -r requirements.txt
   ```
   #### Option B: Install manually
   ```bash
   pip install opencv-python pyautogui mediapipe
   ```

> ⚠️ PyAutoGUI controls your actual mouse — be careful during testing.

## ▶️ How to Run

```bash
python main.py
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


## 🤖 Future Improvements

- Calibration step to auto-detect blink threshold.
- Multi-eye detection for left/right blink actions.
- Drag-and-drop or scrolling based on facial gestures.

## 🙋‍♂️ Author
### Sharavanan Mathivanan
#### GitHub: https://github.com/DiamondDolby
#### LinkedIn: https://www.linkedin.com/in/sharavanan-mathivanan/
