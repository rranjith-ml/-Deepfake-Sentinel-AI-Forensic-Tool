🛡️ Deepfake Sentinel: AI-Powered Forensic Verification
Deepfake Sentinel is a full-stack Machine Learning application designed to assist law enforcement and cybercrime investigators in identifying AI-generated manipulated media. By leveraging state-of-the-art Deep Learning architectures, the system provides real-time analysis, metadata extraction, and forensic reporting.

🚀 Key Features
AI-Powered Detection: Uses a high-performance EfficientNet-B0 model to identify pixel-level inconsistencies and facial artifacts.

Forensic Metadata Analysis: Automatically extracts EXIF data to check for camera source, timestamps, and software modification traces.

Confidence Scoring: Provides a percentage-based reliability score (e.g., "98.4% Probability Fake") to assist in legal documentation.

Real-Time Dashboard: A clean, intuitive interface built with Streamlit for rapid evidence processing.

📊 Technical Performance
The model was trained using Transfer Learning on the Celeb-DF v2 dataset, achieving high convergence and stability.

Final Training Loss: 0.0256

Optimization: Stochastic Gradient Descent (SGD) with a learning rate of 0.001.

Input Resolution: 224x224 pixels.

🛠️ Tech Stack
Language: Python 3.9+

Deep Learning: PyTorch, timm (PyTorch Image Models)

Frontend: Streamlit

Data Processing: OpenCV, PIL, NumPy

Forensics: ExifRead

⚙️ Installation & Usage
Clone the Repository:

Bash
git clone https://github.com/YOUR_USERNAME/Deepfake-Sentinel.git
cd Deepfake-Sentinel
Install Requirements:

Bash
pip install -r requirements.txt
Run the Application:

Bash
streamlit run app.py
🏗️ System Architecture
The system follows a 4-step processing pipeline:

Ingestion: User uploads an image via the web dashboard.

Preprocessing: The image is normalized and resized to match the EfficientNet input requirements.

Inference: The AI model analyzes the facial features for GAN-generated artifacts.

Reporting: Results are displayed alongside extracted metadata and a confidence report.

⚖️ SDG Alignment
This project contributes to SDG 9: Industry, Innovation, and Infrastructure by building resilient digital forensic tools and upgrading the technological capabilities of law enforcement institutions to handle modern AI-driven threats.
