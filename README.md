![Screenshot (66) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/c1811f69-236b-44af-b8e9-6ff10c5ca1a8)# TRANG WEB HỖ TRỢ TẠO THỜI KHÓA BIỂU (CTU) 🌸

Tên website: CAMELLIA TIMETABLE

Niên luận cơ sở ngành kỹ thuật phần mềm (CT239).

Sử dụng framework VueJS và nền tảng Firebase để hỗ trợ authentication, lưu trữ và kết nối realtime tới database, và cả hosting.

## :sunflower: Link website
### :cherries: Trang web cho client
http://camelliatimetable.web.app

## :sunflower: Cài đặt

```bash
# install dependencies
npm install

# Client app and Admin app
npm run dev
```
## :sunflower: Các collections trong CSDL
- subjects
- users

## :sunflower: Một số chức năng chính
### :cherries: Trang web cho client
-	Đăng kí, đăng nhập.
-	Thay đổi mật khẩu.
-	Chọn môn học.
-	Yêu cầu môn học.
-	Lọc nhóm theo điều kiện.
-	Xem thời khóa biểu.
-	Chọn thời khóa biểu yêu thích.
-	Tải ảnh thời khóa biểu đã chọn.
![client_chuc_nang](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/c91df2c5-2ffe-4187-8d90-cd2c26186961)


### :cherries: Trang quản trị cho admin
-	Đăng nhập.
-	Thay đổi mật khẩu.
-	Quản lý môn học (thêm, cập nhật, xóa).
-	Xử lý yêu cầu thêm môn học của người dùng.
-	Quản lý người dùng (xem thông tin người dùng, xóa người dùng)
![admin_chuc_nang](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/6466b2ff-04c3-434e-823d-1bd6fdaf6bf3)


## :sunflower: Hướng dẫn sử dụng chi tiết
### :cherries: Trang web cho client
#### 🍎 Trang đăng nhập, đăng kí:
- Giao diện trang chủ khi chưa đăng nhập, bấm chọn vào biểu tượng đăng nhập.
![1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/e8acd9bb-fc4a-4241-b498-914b1251ac3b)

- Có thể đăng nhập bằng Google bằng cách chọn nút đăng nhập bằng Google:
![2](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8245e24c-0c74-41cb-9e23-9ea8e2f6622f)

-	Sau đó chọn tài khoản đăng nhập:
![3](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/4a6fc700-2f02-4b49-a1df-c49e38a9de4a)

-	Hoặc có thể đăng kí tài khoản mới:
![Screenshot (59)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/63b5bd8a-e646-4ba3-bd31-7f47066b3f96)

-	Sau đó đăng nhập vào bằng tài khoản vừa đăng kí:
![Screenshot (60) - 0](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/1e450ae7-1045-4e7a-bc4b-7b972f45adf1)

-	Thông báo đăng nhập thành công:
![Screenshot (60) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/844dc888-b08d-4ba5-9f9c-887c235586d1)

#### 🍎 Trang chủ:
-	Giao diện trang chủ: hiển thị danh sách tất cả môn học đã có trong cơ sở dữ liệu để người dùng có thể thêm vào danh sách môn cần học. Nhóm nào có sỉ số còn lại lớn hơn 0 sẽ được tô màu xanh lá để người dùng có thể dễ dàng theo dõi. Người dùng có thể ẩn bớt danh sách nhóm của tất cả các môn, chỉ hiển thị mã môn và tên môn bằng cách nhấn vào nút biểu tượng mũi tên hướng lên:
![Screenshot (61) - 0](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/2d6329c9-d39e-4b45-8b29-9da20cacaf4b)

-	Kết quả hiển thị như sau, người dùng cũng có thể hiển thị lại các nhóm như ban đầu bằng cách nhấn vào nút biểu tượng mũi tên hướng xuống:
![Screenshot (61) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/bbec02bb-5f99-4743-a62e-fb3e64ba3e8f)

-	Kết quả như sau, hoặc có thể thu gọn hoặc mở rộng một môn tùy ý bằng cách nhấn chọn biểu tượng tương ứng ở cột tùy chọn của môn đó:
![Screenshot (61) - 2](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8c683334-261a-4b64-bea8-4f61a5334913)
![Screenshot (62)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/e5d101f2-ca0d-4f5f-91b9-a5f75fba9607)

-	Người dùng có thể thêm một môn học vào danh sách môn cần học bằng cách tích chọn vào ô thêm môn ở cột tùy chọn:
![Screenshot (63) - 0](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/1ab14f83-3488-4e47-af89-29cf4c36f095)

-	Thông báo thêm môn thành công:
![Screenshot (63) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/723a6b67-2d0b-44d3-b1d6-5e55c6aac19e)

#### 🍎 Trang các môn cần học:
-	Người dùng cũng có thể thêm môn ở trang môn đã chọn bằng cách nhập mã môn vào ô tìm kiếm, nếu môn đó đã có sẵn trong cơ sở dữ liệu thì kết quả tìm kiếm sẽ hiện ra lập tức.
![Screenshot (64)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/2c239968-3246-4df4-af72-7a15a5465e38)

-	Nhấn vào nút thêm môn để xác nhận thêm môn.
![Screenshot (65)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8f5c5f6e-6940-4805-a3a3-458f66365fdc)

-	Thông báo thêm môn thành công:
![Screenshot (66) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/90e5de76-4bbb-4a90-aa67-02e56e26ca8b)

-	Nếu môn học cần tìm chưa có trong cơ sở dữ liệu, một thông báo môn học chưa có sẽ hiển thị và gợi ý người dùng gửi yêu cầu thêm môn cho admin. Người dùng cần bấm chọn nút “Gửi yêu cầu”.
![Screenshot (66) - 3](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8663b497-9121-4ec0-a34b-8b66a2d5c443)

-	Thông báo đã gửi yêu cầu. Người dùng có thể xem danh sách các môn mình đã yêu cầu bằng cách bấm chọn biểu tượng hình cái chuông ở trên thanh điều hướng. Mặc định, chuông này sẽ đứng yên, nhưng khi có yêu cầu thêm môn nào đó của người dùng đã được duyệt, chuông sẽ rung để thông báo cho người dùng biết.
![Screenshot (66) - 4](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/999bb1b2-03f4-4c55-8ed8-7d34d482e81b)

-	Danh sách yêu cầu người dùng đã gửi:
![Screenshot (66) - 5](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/e7cb8734-00a1-458e-a7fc-ee60911bbd3a)

-	Sau khi đã thêm các môn học, người dùng có thể thêm điều kiện lọc nhóm cho các môn, nhằm lọc ra các nhóm sao cho phù hợp với nhu cầu và sở thích của người dùng. Hình dưới là kết quả lọc theo buổi:
![Screenshot (68)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/f2cbf871-af5f-4837-b983-e38220246d59)

-	Hoặc lọc theo nhóm:
![Screenshot (69)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/f4c9ce47-e255-4ba1-b1de-bdcca451fb36)
![Screenshot (70)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/2659a1e4-66ad-40e6-9202-deb16edc7671)

-	Người dùng có thể xóa môn học, nếu thấy không muốn học môn đó nữa:
![Screenshot (71)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/43a97315-4d6b-4061-940c-dae533904661)
![Screenshot (72)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/d93d56d2-cb48-4be3-a71c-6ef8cddb1b7d)

-	Thông báo xóa môn thành công:
![Screenshot (73)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/0725c670-481c-458d-8bc3-86b024f6bb76)

-	Sau khi đã chọn môn và lọc nhóm, chuyển đến trang thời khóa biểu:
![Screenshot (74)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/b0b4ca5e-cc22-459d-9c89-56805fffac15)

#### 🍎 Trang thời khóa biểu:
-	Với các môn đã chọn và điều kiện lọc nhóm đặt ra, hiện tại chỉ có 1 thời khóa biểu thỏa tất cả các điều kiện đã đề ra.
![Screenshot (75)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/83a3c0b2-7236-4581-abc5-5646c469a59e)

-	Nếu cảm thấy có quá ít lựa chọn, người dùng có thể quay trở lại trang “Môn đã chọn” và bỏ bớt một số điều kiện lọc:
![Screenshot (78)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/b18ab6eb-7c39-4a17-9e00-52035693ad56)

-	Quay trở lại trang thời khóa biểu, lúc này đã có 2 thời khóa biểu thỏa điều kiện.
![Screenshot (79)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/e00f31f8-7918-41d0-8f02-cc88e6e60386)

-	Nếu thấy vừa ý một thời khóa biểu nào đó, người dùng có thể thêm vào yêu thích để cân nhắc sau đó. Có thể chọn yêu thích nhiều thời khóa biểu.
![Screenshot (80)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/c7f34581-76b8-40e0-99d2-9acf4ede2aed)
![Screenshot (81)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/36cc80ce-d69b-4043-81f4-2ee0c237d4ea)

-	Hoặc nếu muốn chọn một thời khóa biểu nào đó làm thời khóa biểu chính thức, người dùng bấm chọn “Chọn làm TKB chính thức”. Lưu ý, chỉ có thể chọn 1 thời khóa biểu làm thời khóa biểu chính thức.
![Screenshot (82)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/11cadd93-74d7-477e-b3ee-522cd99c53d8)
![Screenshot (83)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/7bc2bd08-2ef5-4d8c-b411-d3aed02bb34f)

#### 🍎 Trang thời khóa biểu chính thức:
-	Sau khi chọn thời khóa biểu chính thức ở trang “Thời khóa biểu”, thời khóa biểu đó sẽ được hiển thị bên trang “Đã chọn”. Người dùng có thể xem ảnh chụp màn hình trước khi tải xuống:
![Screenshot (84)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/b11346ca-bd88-43a5-9b45-7c970be98ce6)

-	Bấm chọn “Tải hình ảnh” để tải hình ảnh xuống.
![Screenshot (85)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8643c0d4-1358-4ddd-a707-8863f6a91831)

-	Hình ảnh đã được tải thành công.
![Screenshot (86)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/28e9687c-8bde-4d68-b1b7-40db2ec932e4)

#### 🍎 Chức năng hiển thị thông tin và thay đổi mật khẩu:
-	Sau khi đăng nhập, người dùng có thể xem thông tin cá nhân của mình:
![Screenshot (92)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8f27ca52-6d45-4a67-bf46-4997ca191f5f)

-	Kết quả hiển thị như sau, sau đó người dùng cũng có thể chọn chức năng thay đổi mật khẩu:
![Screenshot (94)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/92e799cf-708c-4b1a-a46d-67dca0bb036c)

-	Nhập vào địa chỉ email để nhận link đổi mật khẩu:
![Screenshot (95)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/51e6b789-2215-4cd2-9d2e-350459fb4940)

-	Thông báo link đổi mật khẩu đã được gửi vào địa chỉ vừa nhập.
![Screenshot (96)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/075d942e-fd7b-4e27-b1fc-b814fee758a7)

-	Vào hộp thư kiểm tra, đi tới đường dẫn được gửi tới.
![Screenshot (97)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/d7c8ffa9-082f-4aad-adcf-64779b1e384b)

-	Nhập vào mật khẩu mới, sau đó bấm chọn “Save”.
![Screenshot (98)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/0d73913f-b2a6-4b4c-9f71-147945c641dd)

-	Thông báo thay đổi mật khẩu thành công.
![Screenshot (99)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/33d14b19-43b8-47d0-9e62-b6c9d77ce6b6)

### :cherries: Trang quản trị cho admin
#### 🍎 Trang đăng nhập:
-	Giao diện trang đăng nhập: admin có thể đăng nhập vào bằng tài khoản google (đã được cấp quyền) hoặc đăng nhập bằng email và mật khẩu.
![Screenshot (108)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/7116aaab-745a-4136-82bc-70f364cb0a3b)

-	Đăng nhập vào bằng tài khoản người dùng thường sẽ có thông báo không có đủ quyền truy cập:
![Screenshot (109) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/94a1f43f-4cb4-4da4-8a0d-b51500ab7e52)

-	Hoặc khi đăng nhập bằng tài khoản admin nhưng sai mật khẩu:
![Screenshot (109) - 2](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/0cd7ff65-db32-421c-a339-98892097e04b)

-	Khi nhập đúng email và mật khẩu, trang web sẽ hiện thông báo đăng nhập thành công:
![Screenshot (110)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/e913966e-96d7-464e-888b-9c4757ed5ebb)

#### 🍎 Trang quản lý tất cả môn học:
-	Trang này hiển thị thông tin tất cả các nhóm của các môn, tương tự như trang người dùng, ta có thể mở rộng và thu gọn các nhóm cho dễ nhìn, nhóm nào có sỉ số lớn hơn 0 cũng được tô màu xanh cho nổi bật. Ngoài ra, trang này còn có cột “Số chọn” nhằm thống kê số người dùng thêm môn học nào đó vào danh sách môn cần học. Admin có thể cập nhật một môn học bằng cách bấm chọn nút “Cập nhật” ở cột tùy chọn tương ứng:
![Screenshot (112)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/4065c778-91e1-4b97-b95f-d0ad4f0bf3fc)

-	Thông báo cập nhật môn học thành công:
![Screenshot (113)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/59803ee9-4a7e-4f02-9ac2-acbf8934c2bf)

-	Hoặc cũng có thể cập nhật lại tất cả các môn, trang web sẽ cập nhật lần lượt từng môn học và thông báo thành công khi cập nhật xong.
![Screenshot (114)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/00c5bea2-ae21-4029-9dac-2aa437f45f4f)
![Screenshot (115)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/58e0a8b0-1dfa-4f85-8d8c-3fa6fedeaa2c)

-	Nếu có môn nào đó không có người dùng nào chọn, admin cũng có thể xóa môn học đó:
![Screenshot (116)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/1b4455f1-dca2-45a4-912f-c2b8fbb251a8)

-	Thông báo xóa môn thành công:
![Screenshot (117)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/d9475aca-8f2b-458a-aa55-378accea1639)

#### 🍎 Trang thêm môn học:
-	Giao diện trang thêm môn học:
![Screenshot (119)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/2149ab34-2d00-49c4-b0cf-4042d4ed0969)

-	Thêm môn tùy ý bằng cách nhập mã môn, sau đó bấm chọn nút “Tìm”:
![Screenshot (120)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/1804e2d1-43c3-4e4c-beaa-13bcacdf6c39)

-	Thông tin môn học cần tìm sẽ hiện ra, sau đó bấm chọn nút “Thêm môn” để xác nhận việc thêm môn:
![Screenshot (121)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/cbe0cae8-0e6e-494b-9d05-3db2ef143024)

-	Thông báo thêm môn thành công:
![Screenshot (122) - 0](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/428e4019-84a1-44a5-8542-191a6753e141)

-	Giả sử admin nhập mã môn nào đó không tồn tại:
![Screenshot (122) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/fdcc5b25-7139-475a-aa56-7aff470591da)

-	Trang web sẽ thông báo không tìm thấy môn học nào:
![Screenshot (122) - 2](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/9715f54f-f9ac-424b-8b18-f306969a1a27)

-	Hoặc admin cũng có thể thêm môn học dựa vào yêu cầu thêm môn của người dùng: khi có yêu cầu gửi tới, biểu tượng chuông trên thanh điều hướng sẽ rung để thông báo cho admin biết. Admin có thể xử lý yêu cầu thêm môn bằng cách bấm vào biểu tượng tìm kiếm của môn học được yêu cầu:
![Screenshot (123)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/a2d38413-705f-42c8-9152-02476e8e4f4b)

-	Trang web sẽ tự động tìm kiếm môn học:
![Screenshot (124)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/0926c4b2-e5a7-4ec7-a574-7ef802f7e498)

-	Thông tin môn học cần tìm hiện ra, admin bấm chọn nút “Thêm môn” để xác nhận thêm môn:
![Screenshot (126)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/6265e7f9-c6c0-48bd-9034-cf27b3cf1c99)

-	Thông báo thêm môn thành công, yêu cầu thêm môn đó cũng biến mất, đồng thời sẽ gửi thông báo yêu cầu thêm môn đã được duyệt cho người dùng:
![Screenshot (127)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/957c7746-e547-4402-8246-c6ef532622b8)

#### 🍎 Trang quản lý người dùng
-	Trang này hiển thị thông tin tài khoản người dùng:
![Screenshot (128)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/e04b1e44-bef9-406b-980b-90d0a952ea67)

-	Admin có thể xem thông tin chi tiết người dùng:
![Screenshot (129)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/9b8f641d-bc0b-4130-939c-3385faed3b23)

-	Kết quả hiển thị:
![Screenshot (130)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/68755db9-6351-4eb4-a039-b83e8e8092f9)

-	Hoặc có thể xóa tài khoản người dùng:
![Screenshot (131) - 1](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/b5e3e5e3-0c2a-4c3f-a7d4-4f36037d0959)
![Screenshot (131) - 2](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/0c3cde71-b37c-421c-a256-9884d7381fc7)

-	Thông báo xóa tài khoản thành công:
![Screenshot (131) - 3](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/95bc0524-aaaf-45f6-9ed7-2da6b8865583)

#### 🍎 Chức năng hiển thị thông tin và thay đổi mật khẩu:
-	Chức năng này tương tự như chức năng của trang người dùng:
![Screenshot (132)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/8acffd93-52b5-4bdc-a116-d5996c64f60c)

-	Cho phép hiển thị thông tin chi tiết của admin hoặc có thể thay đổi mật khẩu nếu muốn:
![Screenshot (133)](https://github.com/HoHongYen/CT239_Timetable_Scheduling/assets/94109674/2819dbef-8cf5-491c-9906-6a0f5bbebb3a)
