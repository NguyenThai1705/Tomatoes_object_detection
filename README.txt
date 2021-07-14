**Tên project: Phát hiện cà chua trực tuyến

--------Các công đoạn huấn luyện ----------------
#1: Chú thích ảnh bằng LabelImg:
**Link tải: https://github.com/tzutalin/labelImg
 - B1: Tạo thư mục Picture trong thư mục chính,
đưa tất cả ảnh cần chú thích vào đó.
 - B2: Cài đặt môi trường theo link hướng dẫn.
 - B3: Khởi động chương trình labelImg.py bằng
Anaconda Prompt.
 - B4: Chọn thư mục Picture vừa tạo làm thư mục
output của file .xml
 - B5: Load tập ảnh trong thư mục Picture và thực
hiện việc đánh Bounding box.

#2: Lưu ảnh và tập chú thích lên Roboflow
**Link upload: https://roboflow.com/
 - B1: Đăng nhập bằng tài khoản google.
 - B2: Chọn Create New Project.
 - B3: Điền tên Project, Loại Project (Object 
Detection Bounding Box), số lớp phân loại.
 - B4: Chọn Create Project.
 - B5: Upload toàn bộ hình ảnh và .xml file.
 - B6: Chọn export dưới dạng COCO format và nhận
đường link.

#3: Huấn luyện trên google colab:
 - B1: Chạy hết tất cả các ô của phần #Install
TensorFlow2 Object Detection Dependencies, lưu ý
ô thứ 2 (%%bash) phải chạy 2 lần.
 - B2: Ở phần #Prepare Tensorflow 2 Object 
Detection Training Data đưa và đường dẫn tải 
tập dữ liệu và chú thích đã tạo bằng công cụ 
Roboflow.
 - B3: Chạy các ô trong phần #Train Custom TF2 
Object Detector rồi đợi kết quả huấn luyện.

--------Các công đoạn chạy đánh giá ----------------
**Giới thiệu tóm tắt:
 - Sử dụng thư viện tensorflow cùng với kiến
trúc mạng học sâu retinanet để phát hiện quả
cà chua trong video hoặc trực tuyến bằng cách 
phát hiện cà chua trên từng khung hình.

** Điều kiện tiên quyết: 
 - Google colab (có GPU) để chạy code.
 - Google drive để lưu dữ liệu input/output.
 - Có video để nhận diện cà chua.
 - Tải thư mục training_demo để nhận trọng số đã được huấn luyện 
   (để đúng tên training_demo và đường dẫn /content/gdrive/My\ Drive/training_demo).

** Các bước thực hiện code:
 1. Chạy hết code cài đặt thư viện phần #Install
TensorFlow2 Object Detection Dependencies và 
bỏ qua phần #Prepare Tensorflow 2 Object 
Detection Training Data vì phần này dùng để huấn
luyện trọng số.

 2. Tạo thư mục Video trên drive của bạn và đưa
video (.mp4) cần phát hiện cà chua vào trong đó.

 3. Chạy hết code phần #Run Inference on Test 
Images with Custom TensorFlow2 Object Detector

 4. Kiểm tra lại thư mục Video để nhận video đã
phát hiện cà chua, hoặc bạn cũng có thể xem trực 
tiếp trên google colab.


-----THANK YOU!-----



