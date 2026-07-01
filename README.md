# AI Image Detection - Nhóm 3T

Dự án phát hiện ảnh do AI tạo ra (AI-generated image detection), so sánh nhiều mô hình: EfficientNet, ResNet50, ViT-B/16, SVM, XGBoost, và mô hình Ensemble.

## Cấu trúc thư mục

```
├── AI_Image_Detection_Nhom3T.ipynb   # Notebook chính (huấn luyện + đánh giá)
├── BaoCao_PhatHien_Anh_AI_Nhom3T.docx # Báo cáo
├── BaoCao_PhatHien_Anh_AI_Nhom3T.pptx # Slide thuyết trình
├── img fake/                          # Ảnh mẫu FAKE
├── img real/                          # Ảnh mẫu REAL
└── results/
    ├── efficientnet/   # metrics, confusion matrix, roc curve, weights, probs
    ├── resnet50/
    ├── vit/
    ├── svm/
    ├── xgboost/
    └── ensemble/
```

## Kết quả tóm tắt

| Model | Accuracy | ROC-AUC |
|---|---|---|
| ViT-B/16 | ~98.5–98.8% | ~0.999 |
| (xem chi tiết trong từng `metrics.json`) | | |

## Lưu ý về file lớn

Các file trọng số mô hình sau **không** được lưu trong repo này (vượt giới hạn 100MB của GitHub):
- `results/vit/vit_weights.pth`
- `results/svm/svm_model.joblib`
- `results/resnet50/resnet50_weights.pth`

👉 Tải các file này tại: *(thêm link Google Drive / Kaggle / Hugging Face Hub của bạn ở đây)*

## Bảo mật

File `kaggle.json` chứa API key cá nhân đã được loại bỏ khỏi repo. Nếu bạn clone project, hãy tự thêm file `kaggle.json` của mình (không commit lên git).
