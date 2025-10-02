# 🛰️ Change Detection of Satellite Imagery Using Deep Learning  

This project implements a **deep learning-based change detection system** for satellite imagery.  
It leverages advanced models like **U-Net, CNNs, and Siamese Networks** to identify changes in land cover, vegetation, urban areas, and other geographical features across different timeframes.  
The system is deployed using **Flask** with a simple web-based interface.  

---

## 🚀 Features
- ✅ Automated change detection from satellite images  
- ✅ U-Net based segmentation model for pixel-wise detection  
- ✅ Web interface for uploading satellite image pairs  
- ✅ Generates:
  - Change masks (highlighting modified regions)  
  - Land vs. Water percentage calculation  
- ✅ Handles noise, lighting variations, and seasonal differences effectively  

---

## 📂 Project Structure
```
├── app.py # Flask app (routes, file uploads, UI handling)
├── server.py # Deep learning model & workflow
├── static/ # Uploaded files, model, and result masks
│ ├── uploads/
│ └── model/satellite_unet.hdf5
├── templates/ # HTML templates (UI)
│ ├── index.html
│ ├── results.html
│ └── layout.html
└── README.md
```

---

## ⚙️ Requirements

### Hardware
- Minimum: 8 GB RAM, Intel i5 / AMD Ryzen 3  
- Recommended: NVIDIA GPU with CUDA support  

### Software
- **OS**: Windows / Linux  
- **Language**: Python 3.8+  
- **Libraries**:  
  - Flask  
  - TensorFlow / Keras  
  - NumPy, Pandas, Matplotlib  
  - PIL, OpenCV  

---

## 🛠️ Installation & Setup
1. Clone the repository:
```bash
git clone https://github.com/SohiniSangoju/ChangeDetectionInSatelliteImageryUsing-DeepLearning.git
cd ChangeDetectionInSatelliteImageryUsing-DeepLearning
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Place the pretrained model in:
```bash
static/model/satellite_unet.hdf5
```

5. Run the Flask app:
```bash
python app.py
```

6. Open your browser and go to:
```bash
http://127.0.0.1:8080/
```

## 📊 Example Results

- Upload a satellite image  
- System generates:  
  - 🖼️ Change mask (highlighting modified regions)  
  - 📊 Land and water distribution percentages  

**Example Output:**  
- 🌊 Water: `36.5%`  
- 🏞️ Land: `63.5%`  
- 🖼️ Change mask saved as `static/mask.png`  

---

## 🔬 Applications

- 🌱 Environmental Monitoring – deforestation, water body shrinkage  
- 🏙 Urban Planning – city expansion tracking  
- 🌾 Agriculture – crop and soil monitoring  
- 🌊 Disaster Management – flood/earthquake impact assessment  

---

## 📌 Future Enhancements

- 📈 Integration with temporal data for predictive change detection  
- 🌈 Support for multispectral & hyperspectral images  
- ☁️ Cloud deployment for real-time monitoring (AWS/GCP)  
- 🗺 GIS integration for spatial decision-making  
- 🤖 Explainable AI (XAI) for interpretable results  

---

## 👨‍💻 Authors

- **S.V.S. Sohini**  
- **T. Swetha** 
- **T. Keerthini**  

---

## 📚 References

- Daud et al., *IEEE Access* 2019 – Change Detection in Remote Sensing Images Using Deep Learning  
- Zhang & Xu, *Remote Sensing* 2020 – Deep Learning Approach to Change Detection in Remote Sensing Images  
- Peng et al., *Remote Sensing* 2019 – End-to-End Change Detection for High Resolution Satellite Images  
- Liu et al., *Remote Sensing* 2020 – Building Change Detection with Siamese Convolutional Network  

