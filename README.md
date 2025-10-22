
# KD-Vocodec

Official audio demonstration website for **KD-Vocodec: A Low-Complexity Model For Joint Speech Coding And Enhancement Using Knowledge Distillation**.

📄 **Paper**: Submitted to ICASSP Workshop 2026
🏆 **Achievement**: Ranked 2nd in ICASSP 2025 Low-Resource Audio Codec (LRAC) Challenge Track 2
🌐 **Live Demo**: [https://yangxu212.github.io/KD-Vocodec/](https://yangxu212.github.io/KD-Vocodec/)

## About KD-Vocodec

KD-Vocodec is a neural speech codec that achieves joint speech coding and enhancement through feature-level knowledge distillation. Our approach employs a teacher-student framework where a compact student encoder learns to reconstruct clean speech representations from noisy inputs by mimicking a pre-trained teacher encoder.

### Key Highlights

- **Low Complexity**: 1.28G MACs | 12.65M parameters
- **Low Latency**: 30ms algorithmic latency
- **Scalable Bitrates**: 1-6 kbps
- **Robust Performance**: Built-in noise suppression and dereverberation
- **No Pre-trained Models**: Trained from scratch without external dependencies

### Technical Innovation

Unlike conventional cascaded enhancement-then-coding pipelines, KD-Vocodec performs enhancement at the feature level before quantization. This ensures that the limited codebook capacity is dedicated to encoding speech content rather than noise patterns, resulting in superior reconstruction quality and robustness at ultra-low bitrates.

## Demo Content

This website showcases audio samples demonstrating KD-Vocodec's performance across different conditions:

- **Bitrates**: 1 kbps (ultra-low) | 6 kbps (low)
- **Acoustic Conditions**: Clean | Noisy | Reverberant
- **Comparison**: Original (degraded) | KD-Vocodec (reconstructed) | Target (clean reference)

## Access the Demo

### 🌐 View Online

The demo website is hosted on GitHub Pages and can be accessed directly:

**[https://yangxu212.github.io/KD-Vocodec/](https://yangxu212.github.io/KD-Vocodec/)**

No installation required - just click and explore!

### 💻 Run Locally

If you prefer to run the demo on your local machine:

1. **Clone the repository**

   ```bash
   git clone https://github.com/yangxu212/KD-Vocodec.git
   cd KD-Vocodec
   ```
2. **Start a local server**

   Choose one of the following methods:

   **Option 1: Python**

   ```bash
   python -m http.server 8000
   ```

   **Option 2: Node.js**

   ```bash
   npx http-server
   ```

   **Option 3: VS Code Live Server**

   - Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
   - Right-click on `index.html` and select "Open with Live Server"
3. **Open in browser**

   Navigate to `http://localhost:8000` (or the port shown in your terminal)

## Project Structure

```
KD-Vocodec/
├── index.html          # Main demo page
├── css/
│   └── style.css      # Styling
├── js/
│   └── demo.js        # Interactive functionality
├── audio/             # Audio samples
│   ├── clean/
│   ├── noisy/
│   └── reverberant/
└── README.md
```

## Authors

**Yang Xu**, **Ronghui Hu**, **Leyan Yang**, **Jing Lu**

*Key Laboratory of Modern Acoustics, Nanjing University*
*NJU-Horizon Intelligent Audio Lab, Horizon Robotics*

📧 **Contact**: lujing@nju.edu.cn

## Citation

If you find our work useful, please cite:

```bibtex
@inproceedings{kdvocodec2025,
  title={KD-Vocodec: A Low-Complexity Model For Joint Speech Coding And Enhancement Using Knowledge Distillation},
  author={Xu, Yang and Hu, Ronghui and Yang, Leyan and Lu, Jing},
  booktitle={ICASSP 2025},
  year={2025}
}
```

## Acknowledgments

This work was supported by the National Natural Science Foundation of China (Grant No. 12274221) and the AI & AI for Science Project of Nanjing University.

## License

© 2025 xuyang Team. For research purposes only.

---

**Enjoy exploring KD-Vocodec! 🎵**
