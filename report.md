# Báo cáo Lab 16: Cloud AI Environment Setup

## 1. Môi trường
- **Instance**: t3.micro (1 vCPU, 1 GB RAM)
- **Region**: us-east-1
- **Thời điểm đo**: 2026-10-03 10:50 UTC

## 2. Dataset
- **Source**: Kaggle - Credit Card Fraud Detection
- **Shape**: 284,807 rows × 31 columns
- **Class distribution**: Normal (0): 284,315 | Fraud (1): 492
- **Load time**: 2.41s

## 3. Kết quả Training
- **Model**: LightGBM
- **Training time**: 3.13s
- **Best iteration**: 1

## 4. Kết quả Evaluation
- **AUC-ROC**: 0.901
- **Accuracy**: 99.92%
- **F1-Score**: 0.763
- **Precision**: 0.754
- **Recall**: 0.772

## 5. Inference Performance
- **Latency (1 row)**: 0.44ms
- **Throughput (1000 rows)**: 1.23M rows/s

## 6. Nhận xét
- Mô hình LightGBM đạt AUC-ROC 0.9 trên t3.micro, cho thấy khả năng phát hiện gian lận tốt
- Inference nhanh (0.44ms/row) phù hợp cho ứng dụng real-time
- Training time ngắn (3.13s) trên CPU cho thấy LightGBM hiệu quả