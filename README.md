#  Adversarial Defense Project: Defending Neural Networks Using Classic and Deep Learning Techniques

Designed a patch attack on real-time camera input, adding patches to the first frame to misclassify
objects. Utilized SuperPoints detector to identify matching points across frames for
consistent patch application.
This project explores multiple defenses against adversarial attacks on image classification models. The techniques range from simple image pre-processing (e.g., JPEG compression, Gaussian blur) to more sophisticated neural network-based approaches like **Autoencoders** and **U-Net**.

##  Defenses Implemented

- **JPEG Compression**: Removes high-frequency adversarial noise.
- **Gaussian Blur**: Smooths out adversarial patterns.
- **Autoencoder**: Learns to reconstruct clean images from perturbed inputs.
- **U-Net**: Trained to denoise adversarial images using semantic segmentation-based architecture.

##  Tools and Libraries Used

- `OpenCV (cv2)` for image processing
- `PyTorch` and `TorchVision` for deep learning models
- `NumPy`, `Matplotlib` for visualization
- `Google Colab` integration for remote model loading
- Custom models: `SIFT`, `SuperPointNet` (for feature robustness evaluation)

##  Folder Structure

```
Adversarial-Defense-Project/
├── Adversarial_Project.ipynb     # Main notebook
├── models/
│   ├── sift.py                   # SIFT feature model
│   └── superpoint.py            # SuperPointNet feature extractor
├── data/                         # Input images or adversarial examples
├── utils/                        # (optional) Helper scripts
├── requirements.txt              # Python dependencies
└── README.md                     # Project overview
```

##  Getting Started

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Run the notebook:

```bash
jupyter notebook Adversarial_Project.ipynb
```

3. Ensure you mount Google Drive if you're using pretrained models stored online.
   https://drive.google.com/drive/folders/1EI0MW_KRz4aXgskkc1owy-g4ffjilK8A?usp=drive_link

##  Example Workflow

1. Load adversarial image.
2. Apply defense: e.g., `jpeg_defense(image)`
3. Visualize or reclassify using robust feature extractors like SIFT or SuperPointNet.

##  Future Directions

- Add benchmarking with accuracy drop before/after defense.
- Extend to adversarial patch attacks or PGD attacks.
- Deploy with a GUI using Gradio or Streamlit.

---

##  Author

**Rishav Kumar**  
**Rahul Kumar**  
For collaborations or questions, feel free to reach out.
