# IoTKITs: A Novel Dataset for IoT Education Kit Recognition

> **Authors**: Thanh-Thien Nguyen, Anh-Tuan Nguyen Do, Duc-Lung Vu
> **Paper**: [ScienceDirect - Data in Brief, June 2025](https://doi.org/10.1016/j.dib.2025.111650)
> **Dataset DOI**: [10.17632/x5thzmkxhy.1](https://data.mendeley.com/datasets/x5thzmkxhy/1)

---

## 📦 Dataset Overview

**IoTKITs** is a well-annotated dataset created specifically for the recognition and classification of **IoT education kits**, including devices like Arduino, ESP32, Raspberry Pi, Jetson Nano, and others commonly used in STEM education.

* 🖼️ **Images**: 3,200 high-resolution RGB images
* 🧷 **Annotations**: JSON format using polygonal masks (via Roboflow)
* 🧠 **Classes**: 32 KIT types (Arduino Uno, Mega2560, ESP8266, Raspberry Pi 5, STM32, etc.)
* 🧪 **Image dimensions**: All resized to 640×640 px for model training
* 🧭 **Sources**: Kaggle, Roboflow Universe, and original photographs

---

## 🎯 Goals and Motivation

While existing PCB datasets focus on components or industrial boards, **IoTKITs** addresses a crucial gap: *complete IoT kit recognition for educational purposes*. The dataset supports the training and benchmarking of object detection models tailored for embedded and classroom environments.

### Key Contributions:

* Rich dataset of full IoT boards used in teaching and research
* Balanced object distribution with realistic backgrounds
* Manual annotations using Roboflow's Smart Polygon Tool for precision

---

## 🧪 Benchmarked Models

| Model        | mAP\@50 | mAP\@50–95 | Parameters (G) |
| ------------ | ------- | ---------- | -------------- |
| YOLOv5       | 0.991   | 0.954      | 0.071          |
| YOLOv7       | 0.987   | 0.956      | 0.374          |
| Faster R-CNN | 0.966   | 0.901      | 0.437          |
| SSD          | 0.929   | 0.750      | 0.279          |

> 🔎 **Observation**: YOLOv5 offered the best trade-off between accuracy and deployability.

---

## 📂 Repository Structure (suggested)

```bash
IoTKITs-dataset/
├── images/              # IoT kit images
├── labels/              # Annotations in JSON or YOLO format
├── dataset.yaml         # Class mappings and dataset config
├── notebooks/           # Sample training/evaluation notebooks
└── README.md
```

---

## 🚀 Quick Start

```bash
# Clone the repo
https://github.com/DoNguyenAnhTuan/IoTKITs-dataset.git

# (Optional) Install requirements
pip install -r requirements.txt

# View samples or run training notebook
cd notebooks/
```

---

## 📜 Citation

Please cite our work if this dataset helps your research:

```bibtex
@article{do2025iotkits,
  title={IoTKITs: A Novel Dataset for IoT Education Kit Recognition},
  author={Nguyen, Thanh-Thien and Do, Anh-Tuan Nguyen and Vu, Duc-Lung},
  journal={Data in Brief},
  volume={60},
  year={2025},
  pages={111650},
  publisher={Elsevier},
  doi={10.1016/j.dib.2025.111650}
}
```

---

## 🧠 License

Dataset licensed under **Creative Commons Attribution 4.0 (CC BY 4.0)**. You may share and adapt with proper attribution.

---

## 📎 Related Resources

* 📘 [Dataset Download - Mendeley Data](https://data.mendeley.com/datasets/x5thzmkxhy/1)
* 🔗 [Portfolio](https://donguyenanhtuan.github.io/AnhTuan-Portfolio/)
* 🎓 Supported by VNU-HCM (DS2024-26-03)
