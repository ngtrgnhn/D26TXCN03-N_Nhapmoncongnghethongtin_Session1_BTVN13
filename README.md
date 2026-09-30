# Bài tập CNTT -- Cyber Arena

## 1. Mục tiêu

Hệ thống hóa kiến thức về: - Các lĩnh vực CNTT và vai trò nghề nghiệp. -
Mô hình IPO (Input -- Process -- Output). - Mô hình DIKW (Data --
Information -- Knowledge -- Wisdom). - Đơn vị lưu trữ, dung lượng và tốc
độ mạng. - Vai trò của CPU, RAM và Storage trong hệ thống.

------------------------------------------------------------------------

## 2. Bối cảnh

Cyber Arena là một trung tâm Gaming & Esports nhỏ, vừa cho khách thuê
máy chơi game, vừa là nơi đội tuyển Liên Minh Huyền Thoại của trường tập
luyện.

Người phụ trách CNTT có các nhiệm vụ: 1. Tuyển người phụ trách kỹ thuật.
2. Thiết kế hệ thống quay và xem lại các trận đấu. 3. Chọn nâng cấp máy
tính.

### Dữ liệu / tài nguyên

-   Mỗi trận đấu tạo ra file log/video có dung lượng khoảng **500 MB**.
-   Đội tuyển thi đấu khoảng **20 trận/tháng**.
-   Trung tâm sử dụng mạng cáp quang **100 Mbps** để livestream lên
    YouTube.
-   Máy chủ game hiện có **16 GB RAM** và **SSD 512 GB**.
-   Ngân sách chỉ đủ tuyển 1 nhân sự kỹ thuật và nâng cấp 1 linh kiện.

### Ràng buộc

-   Dùng mô hình IPO làm xương sống cho hệ thống ghi hình -- xem lại
    trận đấu.
-   `1 Byte = 8 bit`.
-   `1 KB = 1024 Byte`.
-   `1 MB = 1024 KB`.
-   `1 GB = 1024 MB`.
-   `1 TB = 1024 GB`.
-   `Mbps` = Megabit/giây; `MB/s` = Megabyte/giây.
-   Công thức:
    -   `MB/s = Mbps ÷ 8`
    -   `Thời gian (s) = Dung lượng (MB) ÷ Tốc độ (MB/s)`

------------------------------------------------------------------------

# Phần 1 -- Lĩnh vực CNTT và đơn vị lưu trữ

## 1. Chọn nhân sự kỹ thuật

### Ứng viên A

Giỏi lập trình, có thể viết phần mềm dịch vụ thuê máy --- thuộc lĩnh vực
**Kỹ thuật phần mềm**.

### Ứng viên B

Giỏi lắp ráp, sửa máy tính và cài đặt mạng --- thuộc lĩnh vực **Mạng máy
tính / Quản trị hệ thống**.

### Lựa chọn: Ứng viên B

Cyber Arena phụ thuộc nhiều vào máy tính chơi game, hệ thống mạng và
livestream nên cần người có khả năng xử lý phần cứng, mạng và vận hành
hệ thống. Ứng viên B phù hợp hơn với nhu cầu kỹ thuật trực tiếp của
trung tâm, đặc biệt khi chỉ có ngân sách tuyển một người.

## 2. Sắp xếp đơn vị theo thứ tự tăng dần

**Byte → KB → MB → GB → TB**

------------------------------------------------------------------------

# Phần 2 -- Mô hình IPO và lĩnh vực CNTT

## 1. Hệ thống quay lại và xem lại trận đấu theo mô hình IPO

  Thành phần    Trong hệ thống quay/xem lại trận đấu
  ------------- -------------------------------------------------
  **Input**     Tín hiệu video từ camera hoặc màn hình trận đấu
  **Process**   Ghi hình, mã hóa/nén và xử lý video
  **Output**    Video trận đấu được phát lại trên màn hình
  **Storage**   SSD 512 GB lưu trữ video trận đấu

## 2. Hoạt động của Cyber Arena thuộc lĩnh vực CNTT nào?

-   **Livestream:** Mạng máy tính / Quản trị hệ thống.
-   **Quay video:** Kỹ thuật phần mềm / Đa phương tiện.
-   **Xem lại, phát video:** Kỹ thuật phần mềm / Đa phương tiện.

------------------------------------------------------------------------

# Phần 3 -- Tính toán dung lượng và tốc độ mạng

## 1. Tính dung lượng lưu trữ

### a. 20 trận × 500 MB

\[ 20 `\times 500`{=tex} = 10.000 MB \]

Đổi sang GB:

\[ 10.000 `\div 1024`{=tex} `\approx 9`{=tex},77 GB \]

**Kết quả: khoảng 9,77 GB/tháng.**

### b. SSD 512 GB có đủ chứa video của cả tháng không?

Có.

Dung lượng còn trống sau 1 tháng:

\[ 512 - 9,77 = 502,23 GB \]

**Kết quả: còn khoảng 502,23 GB.**

> Bỏ qua dung lượng hệ điều hành và game theo yêu cầu đề bài.

------------------------------------------------------------------------

## 2. Tính tốc độ mạng

### a. 100 Mbps tương đương bao nhiêu MB/s?

\[ 100 `\div 8`{=tex} = 12,5 MB/s \]

**Kết quả: 100 Mbps = 12,5 MB/s.**

### b. Upload video 200 MB mất tối thiểu bao nhiêu giây?

\[ 200 `\div 12`{=tex},5 = 16 giây \]

**Kết quả: tối thiểu khoảng 16 giây.**

### c. Vì sao thực tế thường lâu hơn?

Vì tốc độ 100 Mbps là tốc độ lý thuyết/tối đa. Thực tế còn có hao phí
giao thức mạng, chất lượng đường truyền, máy chủ YouTube, thiết bị mạng
và việc băng thông có thể được chia sẻ cho các thiết bị khác.

------------------------------------------------------------------------

# Phần 4 -- Phần cứng và mô hình DIKW

## 1. Máy chủ chậm khi vừa chạy game vừa livestream

### Lựa chọn: Nâng cấp CPU

Game và livestream đồng thời tạo ra nhiều tác vụ xử lý, đặc biệt là xử
lý và mã hóa video. Máy chủ đã có **16 GB RAM**, nên trong tình huống
này nâng CPU sẽ trực tiếp tăng khả năng xử lý đồng thời các tác vụ và
giảm tình trạng quá tải CPU.

------------------------------------------------------------------------

## 2. Áp dụng mô hình DIKW

**Tình huống:** Huấn luyện viên xem video thấy tuyển thủ hay chết ở phút
15--20, phát hiện họ thiếu tầm nhìn bản đồ, nên yêu cầu mua thêm mắt
(Ward) cho trận sau.

  -----------------------------------------------------------------------
  Tầng DIKW               Nội dung trong tình     Vì sao thuộc tầng này?
                          huống                   
  ----------------------- ----------------------- -----------------------
  **Data**                Tuyển thủ chết ở phút   Đây là dữ liệu/quan sát
                          15--20 trong các        được ghi nhận từ trận
                          video/trận đấu          đấu

  **Information**         Tuyển thủ thường xuyên  Dữ liệu đã được tổng
                          chết ở phút 15--20      hợp thành một xu hướng
                                                  có ý nghĩa

  **Knowledge**           Tuyển thủ thiếu tầm     Đã phân tích và xác
                          nhìn bản đồ             định nguyên nhân của
                                                  vấn đề

  **Wisdom**              Yêu cầu mua thêm mắt    Áp dụng kiến thức để
                          (Ward) cho trận sau     đưa ra quyết định và
                                                  hành động
  -----------------------------------------------------------------------

### Tóm tắt DIKW

**Data → Information → Knowledge → Wisdom**

**Dữ liệu → Thông tin → Kiến thức → Quyết định/Hành động**
