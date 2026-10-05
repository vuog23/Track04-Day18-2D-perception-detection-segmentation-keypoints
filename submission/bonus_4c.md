# Bonus 4C — Val gốc và val lật gương

| Model | Pose mAP50-95 — val gốc | Pose mAP50-95 — val lật gương |
|---|---:|---:|
| flip_idx giải phẫu | 0.4357 | 0.4253 |
| flip_idx đồng nhất | 0.4147 | 0.2751 |

Tập val gốc chỉ có hổ quay phải, nên mAP cao trên tập này không chứng minh model giữ đúng trái/phải giải phẫu khi gặp hổ quay trái. Val lật gương đổi hướng ảnh và hoán đổi nhãn theo FLIP_IDX giải phẫu; mức thay đổi mAP giữa hai tập cho thấy độ nhạy theo hướng, còn so sánh hai model trên val lật gương cho thấy ý nghĩa của quy ước augmentation. mAP là chỉ số tổng hợp, có thể che lỗi ở từng keypoint; cần đọc cùng hình dự đoán và sai số từng điểm.
