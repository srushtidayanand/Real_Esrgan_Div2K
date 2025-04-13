🔍 Real-ESRGAN on DIV2K: Super-Resolution in PyTorch
A simple yet powerful implementation of a super-resolution model using the Real-ESRGAN-inspired architecture trained on the DIV2K dataset.

📌 Features

📦 Dataset Handling – Automated downloading and preprocessing of DIV2K dataset

🧠 Model – Real-ESRGAN inspired model using Residual-in-Residual Dense Blocks (RRDB)

🚀 Training – End-to-end PyTorch training pipeline

📊 Evaluation – PSNR and SSIM metrics for performance

PSNR: 22.75 dB
SSIM: 0.6859

🖼️ Visualization – Side-by-side comparison of LR, SR, and HR images

![image](https://github.com/user-attachments/assets/a01b670a-f02e-478c-8ae2-b7efd4132959)


📁 Project Structure
bash
Copy
Edit
├── real_esrgan_div2k.py     # Main script
├── README.md
└── /content/DIV2K/          # Dataset folder (auto-created)
🔧 Requirements
Python 3.8+
PyTorch
OpenCV
NumPy
tqdm
scikit-image
Matplotlib
requests

Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
🚀 Getting Started
Clone the Repository:

bash
Copy
Edit
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/srushtiddayanand/Real_Esrgan_Div2K/blob/main/real_esrgan_div2k.ipynb)
cd real-esrgan-div2k
Run the Script:

bash
Copy
Edit
python real_esrgan_div2k.py
This will:

Download the DIV2K dataset

Train the model

Evaluate metrics (PSNR, SSIM)

Display sample outputs

🧠 Model Architecture
5 RRDB blocks (each with 3 Residual Dense Blocks)

PixelShuffle upscaling

Final output layer maps to 3 RGB channels

📈 Evaluation Metrics
PSNR (Peak Signal-to-Noise Ratio)

SSIM (Structural Similarity Index Measure)

💾 Model Saving & Loading
The trained model is saved to:
/content/real_esrgan_div2k.pth

Reload and evaluate anytime using:

python
Copy
Edit
model.load_state_dict(torch.load("real_esrgan_div2k.pth"))
🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

📜 License
MIT License

🙌 Acknowledgments
DIV2K Dataset

Real-ESRGAN Paper

PyTorch

