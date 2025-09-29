# 🖥️ Live Video Augmentation 🎨

A simple desktop application that captures live webcam video and applies **real-time visual augmentations**—Grayscale, Sepia, or Sketch—with adjustable brightness, built using Python, OpenCV, NumPy, and Tkinter.

---

## ✨ Features

- **Live Video Feed** from your webcam
- **Augmentation Modes**: None • Grayscale • Sepia • Sketch
- **Brightness Control** via slider
- **Quit Button** to cleanly exit the application

![Live Demo](assets/screenshot.png)

---

## ⚙️ Prerequisites

- **Python 3.7+**
- A working **webcam**

---

## 🚀 Installation

```bash
git clone https://github.com/yourusername/live-video-augmentation.git
cd live-video-augmentation

# (Optional) Create & activate virtual env
python3 -m venv venv
source venv/bin/activate  # macOS/Linux
venv\\Scripts\\activate   # Windows

# Install dependencies
pip install -r requirements.txt
```  

---

## ▶️ Usage

```bash
python app.py
```  

1. **Select** an augmentation mode from the dropdown.
2. **Adjust** brightness using the slider (0–100).
3. **Click** **Quit** to close the window and release the webcam.

---

## 📂 Project Structure

```text
├── app.py             # Main application code
├── requirements.txt   # Python dependencies
└── assets/
    └── screenshot.png # Example screenshot
```

---

## 🛠️ Customization

- **Resolution**: Edit the `cv2.resize()` dimensions in `display_frame()`
- **Augmentations**: Extend `apply_augmentation()` with more filters (e.g., blur, edge detection)
- **GUI Layout**: Modify `create_widgets()` to add more controls

---

## 🐛 Troubleshooting

- **Camera Not Found**: Ensure no other app is using the webcam
- **Tkinter Errors**: On Linux, install via `sudo apt install python3-tk`
- **Performance**: Reduce resize resolution or increase `after()` delay in `update()`

---

## 📜 License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---

## 📝 requirements.txt

```text
opencv-python>=4.5.0
numpy>=1.19.0
```