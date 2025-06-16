```md
# IoTKITs Dataset

**IoTKITs** is a novel, well-annotated dataset designed for identifying and classifying educational IoT kits, including Arduino, Raspberry Pi, ESP32, and more. It enables benchmarking of object detection models in educational and embedded system contexts.

## 📂 Dataset Overview

- **Total Images**: 3,200 RGB images (640×640)
- **Classes**: 32 IoT kit types (e.g., Arduino Uno, ESP32, Raspberry Pi, Jetson Nano)
- **Annotation Format**: Polygon-based labels (JSON or YOLO format)
- **Sources**: Kaggle, Roboflow Universe, custom photos
- **Use case**: Object detection, classification, STEM education AI projects

## 🧪 Benchmark Results

| Model       | mAP@50 | mAP@50–95 | Params (G) |
|-------------|--------|-----------|------------|
| YOLOv5      | 0.991  | 0.954     | 0.07       |
| YOLOv7      | 0.987  | 0.956     | 0.37       |
| Faster R-CNN| 0.966  | 0.901     | 0.43       |
| SSD         | 0.929  | 0.750     | 0.27       |

## 📦 Folder Structure

- `images/` – Dataset images
- `annotations/` – Labels (polygon or YOLO)
- `examples/` – Sample annotated images
- `download_links.txt` – (Optional) Link to Mendeley/Drive for full dataset

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/your_username/IoTKITs.git

# Sample usage with Roboflow or PyTorch
````

## 📝 Citation

If you use this dataset, please cite:

```
@article{nguyen2025iotkits,
  title={IoTKITs: A novel dataset for IoT education kit recognition},
  author={Nguyen, Thanh-Thien and Do, Anh-Tuan Nguyen and Vu, Duc-Lung},
  journal={Data in Brief},
  year={2025},
  publisher={Elsevier}
}
```

[📄 Link to the paper](https://www.sciencedirect.com/science/article/pii/S2352340925003804)

## 🧑‍💻 Authors

* [Anh-Tuan Nguyen Do](https://github.com/DoNguyenAnhTuan) – MSc in IT @ Lac Hong University, FabLab @ EIU
* Collaborators: Thanh-Thien Nguyen, Duc-Lung Vu

## 📜 License

This dataset is released under the **CC BY 4.0** license. You are free to use it for research and educational purposes.

```


