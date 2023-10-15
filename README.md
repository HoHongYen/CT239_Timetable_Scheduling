# TRANG WEB HỖ TRỢ TẠO THỜI KHÓA BIỂU (CTU) 🌸

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
![client_chuc_nang](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/ed8cad3c-5d8c-48e8-a320-02d70f538047)

### :cherries: Trang quản trị cho admin
-	Đăng nhập.
-	Thay đổi mật khẩu.
-	Quản lý môn học (thêm, cập nhật, xóa).
-	Xử lý yêu cầu thêm môn học của người dùng.
-	Quản lý người dùng (xem thông tin người dùng, xóa người dùng)
  
![admin_chuc_nang](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/577cab97-115e-4567-8208-0ca4c53146d5)

## :sunflower: Hướng dẫn sử dụng chi tiết
### :cherries: Trang web cho client
#### 🍎 Trang đăng nhập, đăng kí:
- Giao diện trang chủ khi chưa đăng nhập, bấm chọn vào biểu tượng đăng nhập.
![1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/55b5f7bf-5ee2-4ce0-b6cd-0cccb52a20f0)

- Có thể đăng nhập bằng Google bằng cách chọn nút đăng nhập bằng Google:
![2](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/15a64626-84df-4a93-9f19-67683023f0c7)

-	Sau đó chọn tài khoản đăng nhập:
![3](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/c0cfc10e-3a42-45c9-829d-0f7f564e6bd0)

-	Hoặc có thể đăng kí tài khoản mới:
![Screenshot (59)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/a4d21144-6558-4857-bc7d-f2694c857dab)

-	Sau đó đăng nhập vào bằng tài khoản vừa đăng kí:
![Screenshot (60) - 0](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/0d9dacf6-c0a2-4650-8ce2-94d043ce9d83)

-	Thông báo đăng nhập thành công:
![Screenshot (60) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/cd65d4ee-b352-4103-b4aa-f124ef643650)

#### 🍎 Trang chủ:
-	Giao diện trang chủ: hiển thị danh sách tất cả môn học đã có trong cơ sở dữ liệu để người dùng có thể thêm vào danh sách môn cần học. Nhóm nào có sỉ số còn lại lớn hơn 0 sẽ được tô màu xanh lá để người dùng có thể dễ dàng theo dõi. Người dùng có thể ẩn bớt danh sách nhóm của tất cả các môn, chỉ hiển thị mã môn và tên môn bằng cách nhấn vào nút biểu tượng mũi tên hướng lên:
![Screenshot (61) - 0](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/06031609-5d69-4747-aa9c-acc1da0d3fd3)

-	Kết quả hiển thị như sau, người dùng cũng có thể hiển thị lại các nhóm như ban đầu bằng cách nhấn vào nút biểu tượng mũi tên hướng xuống:
![Screenshot (61) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/178b4103-cc18-42ad-a7bf-1102793d4211)

-	Kết quả như sau, hoặc có thể thu gọn hoặc mở rộng một môn tùy ý bằng cách nhấn chọn biểu tượng tương ứng ở cột tùy chọn của môn đó:
![Screenshot (61) - 2](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/bfec1ec7-9e66-4952-8436-1bcc47f9211e)
![Screenshot (62)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/fa7cf1f7-36ce-4c83-aa76-ab5070de6d88)

-	Người dùng có thể thêm một môn học vào danh sách môn cần học bằng cách tích chọn vào ô thêm môn ở cột tùy chọn:
![Screenshot (63) - 0](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/afefc45b-195a-4577-be5b-2ef0e09682f6)

-	Thông báo thêm môn thành công:
![Screenshot (63) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/af5aed54-a944-4c02-812d-1c5d087b2b64)

#### 🍎 Trang các môn cần học:
-	Người dùng cũng có thể thêm môn ở trang môn đã chọn bằng cách nhập mã môn vào ô tìm kiếm, nếu môn đó đã có sẵn trong cơ sở dữ liệu thì kết quả tìm kiếm sẽ hiện ra lập tức.
![Screenshot (64)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/edbcc1c3-74f5-473c-a8ad-055d409b094b)

-	Nhấn vào nút thêm môn để xác nhận thêm môn.
![Screenshot (65)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/037b1c28-02b4-4f97-ac04-30e427d1d386)

-	Thông báo thêm môn thành công:
![Screenshot (66) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/aa098d44-dbe3-4180-9a90-a246a2313f2a)

-	Nếu môn học cần tìm chưa có trong cơ sở dữ liệu, một thông báo môn học chưa có sẽ hiển thị và gợi ý người dùng gửi yêu cầu thêm môn cho admin. Người dùng cần bấm chọn nút “Gửi yêu cầu”.
![Screenshot (66) - 3](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/5d866a4a-592c-430f-911f-58e36e5bd3cc)

-	Thông báo đã gửi yêu cầu. Người dùng có thể xem danh sách các môn mình đã yêu cầu bằng cách bấm chọn biểu tượng hình cái chuông ở trên thanh điều hướng. Mặc định, chuông này sẽ đứng yên, nhưng khi có yêu cầu thêm môn nào đó của người dùng đã được duyệt, chuông sẽ rung để thông báo cho người dùng biết.
![Screenshot (66) - 4](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/f2ae24aa-ad8f-415c-bf6c-88bb987d06bd)

-	Danh sách yêu cầu người dùng đã gửi:
![Screenshot (66) - 5](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/94968dec-32af-4dd1-9310-84c41e9928c2)

-	Sau khi đã thêm các môn học, người dùng có thể thêm điều kiện lọc nhóm cho các môn, nhằm lọc ra các nhóm sao cho phù hợp với nhu cầu và sở thích của người dùng. Hình dưới là kết quả lọc theo buổi:
![Screenshot (68)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/715bd285-6186-4ad5-890c-974a399c5c66)

-	Hoặc lọc theo nhóm:
![Screenshot (69)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/d9665fb0-002e-4e9d-bec8-e55ab2a0d4f6)
![Screenshot (70)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/2b6cda4a-fe3f-4c50-957f-9679c0518974)

-	Người dùng có thể xóa môn học, nếu thấy không muốn học môn đó nữa:
![Screenshot (71)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/4beff4be-7a37-48fa-8158-16cd10825ae4)
![Screenshot (72)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/22416666-36cb-4d49-9c7d-786d55da289e)

-	Thông báo xóa môn thành công:
![Screenshot (73)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/63c4eeff-f8c3-4a67-a5ae-a769b353b657)

-	Sau khi đã chọn môn và lọc nhóm, chuyển đến trang thời khóa biểu:
![Screenshot (74)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/50445889-a719-474f-bcb7-f8f1631012e6)

#### 🍎 Trang thời khóa biểu:
-	Với các môn đã chọn và điều kiện lọc nhóm đặt ra, hiện tại chỉ có 1 thời khóa biểu thỏa tất cả các điều kiện đã đề ra.
![Screenshot (75)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/b4b7ba48-c338-47e4-8011-2e7f1ee139b5)

-	Nếu cảm thấy có quá ít lựa chọn, người dùng có thể quay trở lại trang “Môn đã chọn” và bỏ bớt một số điều kiện lọc:
![Screenshot (78)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/72c68e6a-dfda-42ed-ba05-7a255fce47dd)

-	Quay trở lại trang thời khóa biểu, lúc này đã có 2 thời khóa biểu thỏa điều kiện.
![Screenshot (79)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/4ac70e9a-a0a4-449a-9102-53c56b6b7d57)

-	Nếu thấy vừa ý một thời khóa biểu nào đó, người dùng có thể thêm vào yêu thích để cân nhắc sau đó. Có thể chọn yêu thích nhiều thời khóa biểu.
![Screenshot (80)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/63e77aeb-ad75-4faa-88fa-a83b8120c495)
![Screenshot (81)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/de2a7f6f-bd34-4888-b79e-34aec0f45bd1)

-	Hoặc nếu muốn chọn một thời khóa biểu nào đó làm thời khóa biểu chính thức, người dùng bấm chọn “Chọn làm TKB chính thức”. Lưu ý, chỉ có thể chọn 1 thời khóa biểu làm thời khóa biểu chính thức.
![Screenshot (82)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/bde88489-64ae-4399-a7af-74bb97c6ef70)
![Screenshot (83)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/3862e4c7-fe88-47ce-a045-67f528c30053)

#### 🍎 Trang thời khóa biểu chính thức:
-	Sau khi chọn thời khóa biểu chính thức ở trang “Thời khóa biểu”, thời khóa biểu đó sẽ được hiển thị bên trang “Đã chọn”. Người dùng có thể xem ảnh chụp màn hình trước khi tải xuống:
![Screenshot (84)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/bc77fa17-af46-4bda-968f-6dfd97cc45d9)

-	Bấm chọn “Tải hình ảnh” để tải hình ảnh xuống.
![Screenshot (85)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/de21b3eb-b0ad-44a0-8630-3c08f1000226)

-	Hình ảnh đã được tải thành công.
![Screenshot (86)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/4699e04f-36c8-49e0-bd1a-98a10bf8923a)

#### 🍎 Chức năng hiển thị thông tin và thay đổi mật khẩu:
-	Sau khi đăng nhập, người dùng có thể xem thông tin cá nhân của mình:
![Screenshot (92)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/93af02d8-4ea1-4122-9fe6-cb5ece2073d0)

-	Kết quả hiển thị như sau, sau đó người dùng cũng có thể chọn chức năng thay đổi mật khẩu:
![Screenshot (94)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/d8d5767a-e4c2-446e-9e4c-fd39d848d497)

-	Nhập vào địa chỉ email để nhận link đổi mật khẩu:
![Screenshot (95)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/c574ff24-e1f6-4957-973c-3255c64a5737)

-	Thông báo link đổi mật khẩu đã được gửi vào địa chỉ vừa nhập.
![Screenshot (96)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/749cbcd1-c8d1-4871-90e5-7018453600df)

-	Vào hộp thư kiểm tra, đi tới đường dẫn được gửi tới.
![Screenshot (97)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/9a64787d-ff01-4122-9321-88a930661341)

-	Nhập vào mật khẩu mới, sau đó bấm chọn “Save”.
![Screenshot (98)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/5c669210-ea77-467d-8d8c-6f1120bb767a)

-	Thông báo thay đổi mật khẩu thành công.
![Screenshot (99)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/e0845ae6-d3ff-4fda-92e5-00da8d2b21b1)

### :cherries: Trang quản trị cho admin
#### 🍎 Trang đăng nhập:
-	Giao diện trang đăng nhập: admin có thể đăng nhập vào bằng tài khoản google (đã được cấp quyền) hoặc đăng nhập bằng email và mật khẩu.
![Screenshot (108)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/d1e33b18-db20-4e62-aff9-0a4844c6de54)

-	Đăng nhập vào bằng tài khoản người dùng thường sẽ có thông báo không có đủ quyền truy cập:
![Screenshot (109) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/fa431302-9800-4556-836f-b172ccfa5a5b)

-	Hoặc khi đăng nhập bằng tài khoản admin nhưng sai mật khẩu:
  ![Screenshot (109) - 2](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/1b2e226e-d19d-4912-8639-ab8faefa8df6)

-	Khi nhập đúng email và mật khẩu, trang web sẽ hiện thông báo đăng nhập thành công:
![Screenshot (110)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/c7e9d441-63ea-4ef1-bafb-5bd528276d0a)


#### 🍎 Trang quản lý tất cả môn học:
-	Trang này hiển thị thông tin tất cả các nhóm của các môn, tương tự như trang người dùng, ta có thể mở rộng và thu gọn các nhóm cho dễ nhìn, nhóm nào có sỉ số lớn hơn 0 cũng được tô màu xanh cho nổi bật. Ngoài ra, trang này còn có cột “Số chọn” nhằm thống kê số người dùng thêm môn học nào đó vào danh sách môn cần học. Admin có thể cập nhật một môn học bằng cách bấm chọn nút “Cập nhật” ở cột tùy chọn tương ứng:
![Screenshot (112)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/f74bef1a-717c-4ea5-bd62-388ea91db396)

-	Thông báo cập nhật môn học thành công:
![Screenshot (113)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/571437e1-f6d8-4405-8d48-292ca73819cb)

-	Hoặc cũng có thể cập nhật lại tất cả các môn, trang web sẽ cập nhật lần lượt từng môn học và thông báo thành công khi cập nhật xong.
![Screenshot (114)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/e5538923-0e34-4a2f-ab0f-826b5709e9d1)
![Screenshot (115)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/7348af5d-71b6-48d6-9595-6759748ec662)

-	Nếu có môn nào đó không có người dùng nào chọn, admin cũng có thể xóa môn học đó:
![Screenshot (116)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/e64fbe77-c533-4dd0-aadf-9edc298b250f)

-	Thông báo xóa môn thành công:
![Screenshot (117)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/29c7b5b0-cd8f-452d-b008-a3a15875d893)

#### 🍎 Trang thêm môn học:
-	Giao diện trang thêm môn học:
![Screenshot (119)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/88434e73-c99f-40e8-9e7b-05c9ed20290f)

-	Thêm môn tùy ý bằng cách nhập mã môn, sau đó bấm chọn nút “Tìm”:
![Screenshot (120)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/1790a6d5-6caf-4d72-9ccd-20da33909e95)

-	Thông tin môn học cần tìm sẽ hiện ra, sau đó bấm chọn nút “Thêm môn” để xác nhận việc thêm môn:
![Screenshot (121)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/75642202-0d5f-4d26-8246-df12e31eab40)

-	Thông báo thêm môn thành công:
![Screenshot (122) - 0](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/f2861d13-9a3c-4ede-9d15-e3ac76bf0ced)

-	Giả sử admin nhập mã môn nào đó không tồn tại:
![Screenshot (122) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/109914b8-43dc-4e32-a109-830925cca2fb)

-	Trang web sẽ thông báo không tìm thấy môn học nào:
![Screenshot (122) - 2](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/b9716c8f-019a-4e9f-ac0a-0dc6b409c28a)

-	Hoặc admin cũng có thể thêm môn học dựa vào yêu cầu thêm môn của người dùng: khi có yêu cầu gửi tới, biểu tượng chuông trên thanh điều hướng sẽ rung để thông báo cho admin biết. Admin có thể xử lý yêu cầu thêm môn bằng cách bấm vào biểu tượng tìm kiếm của môn học được yêu cầu:
![Screenshot (123)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/f2432c98-9cc4-4469-98c1-dd3c19cfe9f3)

-	Trang web sẽ tự động tìm kiếm môn học:
![Screenshot (124)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/3bfbacd4-694e-4028-af7b-182594a97070)

-	Thông tin môn học cần tìm hiện ra, admin bấm chọn nút “Thêm môn” để xác nhận thêm môn:
![Screenshot (126)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/fed033c1-1b8d-495a-8b0d-403f4cdca855)

-	Thông báo thêm môn thành công, yêu cầu thêm môn đó cũng biến mất, đồng thời sẽ gửi thông báo yêu cầu thêm môn đã được duyệt cho người dùng:
![Screenshot (127)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/92b85379-4f78-4a8c-abfc-f093d8dbf0d0)

#### 🍎 Trang quản lý người dùng
-	Trang này hiển thị thông tin tài khoản người dùng:
![Screenshot (128)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/3985213d-e070-4170-ac88-e549331ab5f1)

-	Admin có thể xem thông tin chi tiết người dùng:
![Screenshot (129)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/35abe01b-e809-4313-a73f-6789405df888)

-	Kết quả hiển thị:
![Screenshot (130)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/86c7771c-2adb-4eab-b227-5f9435c1bf90)

-	Hoặc có thể xóa tài khoản người dùng:
![Screenshot (131) - 1](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/2df4e019-5aa9-4296-9897-96a1fa348624)
![Screenshot (131) - 2](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/8e75c0a3-56ee-40d8-bf38-e5336d9a78eb)

-	Thông báo xóa tài khoản thành công:
![Screenshot (131) - 3](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/83490e8b-213f-4e6a-998d-746c88ec7d1f)

#### 🍎 Chức năng hiển thị thông tin và thay đổi mật khẩu:
-	Chức năng này tương tự như chức năng của trang người dùng:
![Screenshot (132)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/d386b544-fbda-468f-9a0e-fca57302fafa)

-	Cho phép hiển thị thông tin chi tiết của admin hoặc có thể thay đổi mật khẩu nếu muốn:
![Screenshot (133)](https://github.com/HoHongYen/Timetable_Scheduling/assets/94109674/0aabb892-f84f-4f15-ada5-7b432d90a8cc)
