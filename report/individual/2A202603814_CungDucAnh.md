# Báo cáo cá nhân — Day 01: Lọc tin nhắn rác bằng ML, DL, Embedding và LLM

> Đổi tên file này thành `MSSV_HoTen.md` của bạn, ví dụ `2A20260000_NguyenVanAn.md`, rồi điền từng mục. Xoá các dòng hướng dẫn in nghiêng khi xong.

- **MSSV:** 2A202603814
- **Họ và tên:** Cung Đức Anh
- **SEED** (in ở ô đầu notebook): 6769

## 1. Bằng chứng

| Tệp | Có? |
| --- | --- |
| [`day01_lab.ipynb`](day01_lab.ipynb) — notebook đã chạy, còn output | ☐ | có
| [`lab1_report.json`](lab1_report.json) — do ô "Báo cáo cuối" sinh ra | ☐ | có
| [`hand_calc.jpg`](hand_calc.jpg) — ảnh tính tay có các bước | ☐ | có

## 2. Kết quả chính

% đoán ĐÚNG theo nhóm case (càng đậm càng tốt)
 	1. BoW + LogReg	2. BoW + MLP	3a. Emb + kNN	3b. Emb + LogReg	3c. Emb + MLP head	4a. LLM nhỏ zero-shot	4d. LLM nhỏ + prompt phòng thủ
false_alarm_keywords	100%	0%	100%	0%	0%	100%	100%
Tưởng spam nhưng không phải	100%	90%	70%	80%	80%	100%	100%
leetspeak_obfuscation	0%	100%	100%	100%	100%	100%	100%
legit_transaction_otp	0%	0%	0%	0%	0%	100%	0%
Thao túng / lừa đảo	12%	25%	88%	50%	50%	100%	100%
meta_spam_talk	0%	0%	0%	0%	0%	100%	100%
Spam giọng tự nhiên	20%	0%	40%	20%	30%	100%	100%
Né từ khoá	17%	17%	83%	83%	67%	100%	100%
phishing_bank	0%	100%	100%	100%	100%	100%	100%
Prompt injection	67%	83%	83%	100%	100%	100%	100%
Nói về spam	100%	100%	25%	50%	50%	100%	100%
Tin giao dịch hợp lệ	67%	83%	100%	83%	67%	100%	100%
TỔNG (50 case)	49%	51%	69%	62%	60%	100%	98%

## 3. Dự đoán và thực tế

*Chọn 3 dự đoán `predict(...)` lệch nhiều nhất so với kết quả. Mỗi cái: bạn đoán gì, ra gì, vì sao lệch.*

## 4. Phân tích 50 case khó

*Model nào tụt nhiều nhất, ở nhóm case nào? Nêu 2 case cụ thể và cơ chế khiến model sai.*

## 5. Thử thách cá nhân

*Đề theo SEED của bạn, cách làm, kết quả, giải thích.*

## 6. Phương án cho sản phẩm thật

*Với yêu cầu p95 < 50 ms/tin cho 10 triệu SMS/ngày: chọn phương án nào, dẫn số liệu nào, chấp nhận đánh đổi gì.*

## 7. AI log và điều đã học

*Mỗi lần dùng AI: hỏi gì, nhận gì, bạn sửa gì. Sau đó 2–3 câu: điều bạn hiểu ra hôm nay mà trước đó chưa hiểu.*

Thật sự là đề bài dài quá em làm cả chiều thêm tối về làm từ 9h vẫn không đủ thời gian hoàn thiện file này mong BTC thông cảm ạ