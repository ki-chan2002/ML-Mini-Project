# Mini-Project for Fundamentals of Machine Learning Course
![background](./materials/ai_wp.jpg)
This repository contains the code and data for a mini-project on facial expression recognition using machine learning algorithms.

## 📑 Project Policy


    |No.| Student Name    | Student ID |
    | --------| -------- | ------- |
    |1|Ngô Châu Xuân Hà|20110173|
    |2|Võ Quang Tuấn|21110438|
    |3|Trần Đăng Khoa|20280054|
    |4|Nguyễn Quốc Dương|20280021|

Phân công công việc (dự kiến)
Hà: phần 1 question 2, chuẩn bị data source cho phần 3, hoàn thành MLP và Logistic Regression
Tuấn: phần 2 question 2 (do chưa sử dụng thạo github nên Hà commit hộ). Viết đánh giá
Khoa: thao tác chính liên quan đến github (merge,...). áp model mẫu cho cho phần 3 dựa theo data source và sử dụng gridsearch
Dương: hỗ trợ Khoa áp model mẫu cho phần 3 dựa theo data source

interesting findings
- Tập này có 2 cách tiếp cận khi scale và pca: áp dụng cho từng ảnh một và áp dụng cho cả tập
- Khi áp dụng cho từng ảnh thì cho vào hàm show_img ảnh tuy bị bể do đã qua xử lý nhưng vẫn giữ được nét đặc trưng
- Khi áp dụng cho cả tập thì cho vào hàm show_img sẽ ra ảnh khác so với xử lý từng ảnh và có vài ảnh bị trùng (mặc dù cùng một hàm show_img)

cho nên là áp dụng cả 2 cách xử lý tập để cho vào model, sẽ dựa vào điểm số để đánh giá cách làm nào tốt hơn

update: loại data đầu vào cho model theo cách 2 là xử lý cho từng ảnh vì tốn nhiều thời gian, thao tác nhiều hơn nhưng không thu lại được gì nhiều. Cụ thể điểm số không đỏi  mà còn thấp hơn

update: cảm ơn Tuấn đã viết phần kết luận chi tiết, Khoa chuyển lại thành tiếng Anh

update: sử dụng gridsearchcv quá mất thời gian cho các model (có model thử trên 540p vẫn chưa xong) nên hướng xử lý khác là tách nhỏ model ra để chạy

update: mặc đù đã đủ 4 model nhưng nhóm vẫn muốn thử thêm naive bayes, hi vọng sẽ ra kết quả tốt hơn