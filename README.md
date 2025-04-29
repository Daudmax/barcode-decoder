# Barcode Decoder 

## Barcode Detection and Decoding System using YOLO 

## 📌 Project Overview

This project builds a system to detect barcodes in images, crop the detected regions, and decode them to reveal the barcode information.

We use YOLOv8 (You Only Look Once) for barcode detection and Pyzbar library for decoding.

---

## 📚 Project Structure

- `Barcode_Decoder_Project_Model_Training.ipynb` → Trains YOLOv8 on custom barcode dataset.
- `Barcode_Decoder_Project_Model_Testing.ipynb` → Tests the trained model and decodes barcodes from test images.
- `dataset ->` "https://drive.google.com/drive/folders/1RoPo4aOoWh_ByNP-WMtlylC7FkpSdxHF?usp=sharing" -> new_dataset → Contains sample images used during training, validation, and testing.
- `README.md` → This file.

---

## 🛠️ Technologies Used

- Python
- Google Colab
- YOLOv8 (Ultralytics library)
- OpenCV
- Pyzbar
- ZBar (barcode scanning library)

---

## 🖼️ Dataset

- Custom barcode dataset created manually from large roboflow dataset
- Divided into `train`, `valid`, and `test` folders.
- Each folder contains:
  - `/images` (actual images)
  - `/labels` (YOLO annotation files)

---

## 🚀 How to Run the Project

1. Open the **Barcode_Decoder_Project_Model_Training.ipynb** notebook.
2. Mount your Google Drive.
3. Unzip dataset and train YOLOv8 model.
4. Save the trained model (`best.pt` or `saved_model.pt`).

Then:

5. Open the **Barcode_Decoder_Project_Model_Testing.ipynb** notebook.
6. Upload your trained model weights either `best.pt` or `saved_model.pt` but `best.pt` has best weights 
7. Upload images for testing.
8. Predict barcode regions, crop, and decode them automatically.

---

## 📈 Model Performance

- Model evaluated using mAP, Precision, Confusion Matrix and Recall metrics.
- Metrics printed during validation step and their images stored in the runs

---

## ⚙️ Requirements

Install the following packages:

```bash
pip install ultralytics pyzbar opencv-python-headless
apt-get update
apt-get install -y libzbar0

```

## 🙋 Author

Keerthana Nehru

Barcode Decoder Project  
April 2025
