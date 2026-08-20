# Nhận diện Mã số Container (Container Code Detection & Recognition)

Dự án phát hiện và nhận diện mã số container đạt độ chính xác cao bằng sự kết hợp giữa **YOLOv8** và **PaddleOCR** / **EasyOCR** / **TrOCR**.

---

## 🚀 Google Colab Notebooks (Huấn luyện & Tinh chỉnh)

Dưới đây là các liên kết mở trực tiếp Notebook từ GitHub lên **Google Colab** để chạy huấn luyện trên GPU miễn phí:

* **Huấn luyện tinh chỉnh nhận diện ký tự (PaddleOCR Fine-tuning):**
  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LongLongoooo/Container_Code_Detection/blob/main/paddleocr_finetuning.ipynb)

* **Huấn luyện phát hiện vùng mã (YOLOv8 Training):**
  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LongLongoooo/Container_Code_Detection/blob/main/Container_Code_Detection.ipynb)

---

## 🛠️ Hướng dẫn Chạy Offline trên Máy Local

### 1. Khởi động Web UI Streamlit
Ứng dụng Web UI hỗ trợ kéo thả ảnh, lựa chọn mô hình OCR (PaddleOCR/EasyOCR/TrOCR) và điều chỉnh ngưỡng tin cậy YOLO.

Để chạy Web UI trên môi trường ảo Python 3.12:
```powershell
# Chạy máy chủ Streamlit
test\venv_312\Scripts\python.exe -m streamlit run app.py
```
Sau khi khởi động, truy cập ứng dụng tại địa chỉ: **[http://localhost:8501](http://localhost:8501)**.

### 2. Chạy Kiểm thử Batch Test (Kiểm tra 11 ảnh mẫu)
Chạy script kiểm thử để kiểm tra độ chính xác và xuất báo cáo kiểm định chuẩn ISO 6346:
```powershell
test\venv_312\Scripts\python.exe test/test_ocr.py
```

---

## 📂 Hướng dẫn mở thủ công Notebook trên Google Colab từ GitHub

Nếu bạn muốn mở thủ công bất kỳ Notebook nào từ GitHub lên Colab:
1. Truy cập trang web: **[Google Colab](https://colab.research.google.com/)**.
2. Một hộp thoại hiện lên, chọn tab **GitHub**.
3. Dán đường dẫn repository của bạn vào ô tìm kiếm:
   `https://github.com/LongLongoooo/Container_Code_Detection`
4. Nhấn **Enter**, hệ thống sẽ liệt kê các file `.ipynb` trong dự án. Bạn chỉ cần click vào tệp cần mở!
