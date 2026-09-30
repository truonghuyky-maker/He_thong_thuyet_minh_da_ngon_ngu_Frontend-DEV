Tourist Guide Pro Newbie

I.	General

Các vấn đề và thách thức gặp phải
•	Thông thường, các khách du lịch nước ngoài khi đi du lịch tại các nước khác họ. Họ thường bị chắn bởi rào cản ngôn ngữ khi giao tiếp với những người bản xứ tại khu du lịch. Và ngược lại đối với người du lịch trong nước đi sang nước ngoài.
•	Đồng thời, các khách du lịch thông thường có rất nhiều câu hỏi trong khi đi du lịch nhưng lại thiếu đi công cụ giúp họ dịch ngôn ngữ, chỉ dẫn và hỗ trợ họ trên con đường du lịch.

Cấp độ hướng đến
•	Xây dựng web quản lý ứng dụng trên mobile, phù hợp với nhiều trình duyệt khác nhau và hệ điều hành (OS) khác nhau.
•	Cho phép người dùng chọn Points of Interest (POIs) và nó có chức năng multilingual text hoặc audio guidance.
•	Có kích hoạt GPS để hiển thị địa điểm khách du lịch/người dùng trên bản đồ.
•	Tích hợp một AI-powered chatbox có khả năng đa ngôn ngữ để trả lời hoặc đáp lại các câu hỏi mà khách du lịch hỏi bằng ngôn ngữ thích hợp với khách du lịch để khách du lịch nghe và hiểu.

Giả sử tình huống
•	Một vị khách du lịch vừa mới đến địa điểm du lịch. Mở ứng dụng lên trên điện thoại. Trên bản đồ trong điện thoại của khách du lịch sẽ xuất hiện các địa điểm bắt khách gần đây, các POIs gần đây và hiển thị vị trí đang đứng của vị khách du lịch ấy.
Khách du lịch nhấn và chọn vào một địa điểm bắt khách nào đấy. Bản đồ sẽ chỉ đường phù hợp và an toàn cho khách du lịch đi đến địa điểm khách chọn.
•	Trên đường khách du lịch đang tham quan, khách có thể nhấn vào POIs để có thể nghe audio thuyết minh về địa điểm mà khách sắp đến và đọc những mô tả về địa điểm du lịch bằng ngôn ngữ mà khách du lịch đề xuất hay chọn để trả lời.
•	Nếu khách du lịch có câu hỏi, khách có thể hỏi chatbox đã được tích hợp trong hệ thống. Chatbox sẽ đáp lại khách du lịch ngay lập tức với thông tin đầy đủ.

Kết quả mong muốn
•	Một hệ sinh thái phần mềm du lịch thông minh đa nền tảng.
•	Hệ thống thuyết minh đa ngôn ngữ linh hoạt (Multilingual Guidance).
•	Trợ lý ảo AI thông minh (AI-powered Chatbot).
•	Điều hướng & Chỉ đường an toàn (Navigation System).
•	Xóa bỏ rào cản ngôn ngữ & Nâng cao trải nghiệm du lịch.

II.	Specific

Actor (s): Admin, Staff, App User

Basic Course of Events (Luồng sự kiện chính)
Step 1
Actor Action: Khách du lịch (Tourist) truy cập ứng dụng/trang web và chọn chức năng xem/tìm kiếm lịch trình du lịch (Search/View Tour).
System Response: Hệ thống hiển thị giao diện tìm kiếm kèm danh sách các tour du lịch phổ biến, danh mục các điểm đến và các bộ lọc tìm kiếm (địa điểm, ngân sách, số ngày, loại hình du lịch).

Step 2
Actor Action: Khách du lịch nhập từ khóa tìm kiếm hoặc chọn các tiêu chí lọc (ví dụ: địa điểm, khoảng giá, ngày khởi hành). [A1]
System Response: Hệ thống ghi nhận các thông tin lọc và tìm kiếm trong cơ sở dữ liệu.

Step 3
Actor Action: 
System Response: Hệ thống hiển thị danh sách các tour du lịch phù hợp với tiêu chí tìm kiếm. [E1]

Step 4
Actor Action: Khách du lịch chọn một tour cụ thể từ danh sách kết quả để xem chi tiết.
System Response: Hệ thống hiển thị thông tin chi tiết về tour: lịch trình từng ngày, địa điểm tham quan, giá tour, thông tin hướng dẫn viên, và các đánh giá (reviews) từ người dùng khác.

Step 5
Actor Action: Khách du lịch chọn "Đặt tour" (Book Tour) và nhập/xác nhận thông tin cá nhân (Họ tên, Email, Số điện thoại, Số lượng người đi). [A2]
System Response: Hệ thống kiểm tra số lượng chỗ còn trống của tour. [E2]

Step 6
Actor Action: Khách du lịch chọn phương thức thanh toán và nhập thông tin thanh toán (Thẻ tín dụng, Chuyển khoản, Ví điện tử). [A3]
System Response: Hệ thống xác thực thông tin thanh toán và tiến hành xử lý giao dịch. [E3]

Step 7
Actor Action:
System Response: Hệ thống lưu thông tin đặt tour vào cơ sở dữ liệu, gửi email/tin nhắn xác nhận đặt tour thành công kèm mã vé/mã đặt chỗ cho khách du lịch và hiển thị màn hình thông báo hoàn tất.
(Luồng sự kiện kết thúc)


Alternative Paths (Luồng sự kiện thay thế)
A1. Tìm kiếm theo đề xuất/Vị trí hiện tại (Location-Based Search)
1.	Khách du lịch bật tính năng truy cập vị trí hiện tại trên thiết bị.
2.	Hệ thống tự động quét và gợi ý các điểm đến hoặc các tour du lịch ngắn hạn xung quanh vị trí của khách du lịch.
3.	Khách du lịch chọn một trong các gợi ý.
4.	Quay lại bước 4 của Basic Course of Events.
A2. Lưu tour vào Danh sách yêu thích (Save to Wishlist)
1.	Tại bước 4 của Luồng chính, thay vì chọn "Đặt tour", Khách du lịch chọn biểu tượng "Thêm vào danh sách yêu thích" (Wishlist/Bookmark).
2.	Hệ thống lưu thông tin tour vào tài khoản cá nhân của khách du lịch và hiển thị thông báo "Đã lưu thành công".
3.	Luồng sự kiện kết thúc tại đây.
A3. Hủy bỏ quá trình đặt tour (Cancel Booking)
1.	Tại bước 5 hoặc 6 của Luồng chính, Khách du lịch chọn nút "Hủy đặt" (Cancel) hoặc quay lại trang chủ.
2.	Hệ thống khôi phục các trạng thái chưa lưu và đưa Khách du lịch trở lại màn hình chi tiết tour hoặc danh sách tour ban đầu.
3.	Quay lại bước 3 hoặc 4 của Basic Course of Events.

Exception Paths (Luồng sự kiện ngoại lệ)
E1. Không tìm thấy kết quả phù hợp (No Results Found)
1.	Tại bước 3 của Luồng chính, nếu cơ sở dữ liệu không tìm thấy tour nào khớp với bộ lọc/từ khóa của người dùng.
2.	Hệ thống hiển thị thông báo "Không tìm thấy tour phù hợp với yêu cầu của bạn", đồng thời đưa ra gợi ý điều chỉnh bộ lọc hoặc đề xuất các tour hot khác.
3.	Quay lại bước 2 của Basic Course of Events.
E2. Tour đã hết chỗ (Tour Sold Out / Out of Seats)
1.	Tại bước 5 của Luồng chính, hệ thống phát hiện số lượng chỗ còn trống nhỏ hơn số lượng vé Khách du lịch đăng ký.
2.	Hệ thống hiển thị thông báo lỗi "Số lượng chỗ còn lại không đủ cho đoàn của bạn" và hiển thị các ngày khởi hành khác còn trống của tour đó.
3.	Quay lại bước 5 của Basic Course of Events.
E3. Lỗi thanh toán / Giao dịch thất bại (Payment Failure)
1.	Tại bước 6 của Luồng chính, nếu số dư tài khoản không đủ, thông tin thẻ không hợp lệ hoặc kết nối cổng thanh toán bị gián đoạn.
2.	Hệ thống báo lỗi "Giao dịch không thành công. Vui lòng kiểm tra lại thông tin thanh toán hoặc thử phương thức khác".
3.	Giữ nguyên thông tin đặt tour đã nhập và cho phép Khách du lịch chọn lại phương thức thanh toán.
4.	Quay lại bước 6 của Basic Course of Events.

Extension Points (Các điểm mở rộng)
Location-Based Recommendation (Gợi ý theo vị trí)
•	Location (Điểm đặt): Tại Bước 2 của Luồng sự kiện chính (Basic Course). 
•	Condition (Điều kiện): Khách du lịch bật định vị GPS và chọn tìm kiếm/đề xuất theo vị trí hiện tại. 
•	Extension (Hành động mở rộng): Hệ thống quét vị trí và tự động gợi ý các POIs (địa điểm tham quan) hoặc các tour du lịch ngắn hạn xung quanh. (Tham chiếu: Alternate Path A1) 
Save to Wishlist (Lưu vào danh sách yêu thích)
•	Location (Điểm đặt): Tại Bước 4 của Luồng sự kiện chính (khi xem chi tiết tour). 
•	Condition (Điều kiện): Khách du lịch nhấn vào biểu tượng "Thêm vào danh sách yêu thích" (Wishlist/Bookmark) thay vì bấm "Đặt tour". 
•	Extension (Hành động mở rộng): Hệ thống lưu thông tin tour vào tài khoản cá nhân của khách du lịch mà không chuyển sang bước thanh toán. (Tham chiếu: Alternate Path A2) 
Multilingual Audio Guidance (Thuyết minh âm thanh đa ngôn ngữ)
•	Location (Điểm đặt): Tại Bước 4 của Luồng sự kiện chính (khi xem chi tiết tour/POIs). 
•	Condition (Điều kiện): Khách du lịch yêu cầu nghe bản thuyết minh âm thanh bằng ngôn ngữ ưu tiên khi đến hoặc xem thông tin về POIs. 
•	Extension (Hành động mở rộng): Hệ thống phát đoạn audio thuyết minh tự động hoặc tải nội dung văn bản dịch tương ứng theo cấu hình ngôn ngữ đã chọn. 
AI-Powered Chatbot Support (Hỗ trợ qua Trợ lý ảo AI)
•	Location (Điểm đặt): Bất kỳ bước nào trong quá trình trải nghiệm/đặt tour. 
•	Condition (Điều kiện): Khách du lịch mở giao diện chat và gửi câu hỏi thắc mắc bằng ngôn ngữ bất kỳ. 
•	Extension (Hành động mở rộng): Chatbot AI nhận diện ngôn ngữ, phân tích câu hỏi và phản hồi thông tin hướng dẫn, giải đáp ngay lập tức. 

Triggers (Tác nhân / Sự kiện kích hoạt)
Người dùng (Khách du lịch) mở ứng dụng/trang web và truy cập vào chức năng Tìm kiếm / Xem lịch trình du lịch (Search/View Tour) hoặc yêu cầu tìm kiếm địa điểm/POIs xung quanh vị trí hiện tại.

Assumptions (Giả định)
Thiết bị & Kết nối: Thiết bị của người dùng có kết nối Internet ổn định; dịch vụ định vị (GPS) đã được bật và được cấp quyền truy cập để ứng dụng hoạt động chính xác các tính năng chỉ đường, POIs. 
Đa ngôn ngữ & Dữ liệu: Dữ liệu về các điểm tham quan (POIs), tệp âm thanh thuyết minh (audio guidance) và các gói tour đã được cập nhật đầy đủ trong hệ thống. 
Hệ thống Chatbot & Thanh toán: Tích hợp thành công mô hình AI Chatbot đa ngôn ngữ và liên kết hoạt động ổn định với các cổng thanh toán trực tuyến (Thẻ, Ví điện tử, Banking). 
Tài khoản người dùng: Người dùng đã đăng nhập (hoặc được định danh tạm thời) để có thể thực hiện đặt tour hoặc lưu vào Danh sách yêu thích (Wishlist).

Preconditions: Không có

Post Conditions (Điều kiện sau khi thực hiện / Kết quả)
Trường hợp thành công (Success End Condition):
•	Thông tin đặt tour được lưu vào cơ sở dữ liệu hệ thống. 
•	Số lượng chỗ trống còn lại của tour được tự động cập nhật (trừ đi số vé vừa đặt). 
•	Hệ thống gửi thông báo xác nhận kèm mã vé/mã đặt chỗ thành công tới người dùng qua Email/SMS. 
•	(Trường hợp Save to Wishlist) Tour đã được lưu thành công vào danh sách yêu thích cá nhân của người dùng. 
Trường hợp thất bại / Hủy bỏ (Failure End Condition):
•	Không có giao dịch hay vé nào được tạo; dữ liệu hệ thống giữ nguyên không bị thay đổi dư thừa. 
•	Người dùng nhận được thông báo lỗi rõ ràng (ví dụ: Hết chỗ, Lỗi thanh toán, Không tìm thấy kết quả) kèm theo hướng dẫn khắc phục hoặc điều hướng quay lại các bước trước. 

Cấu trúc thư mục
my-tourist-app/
├── public/                     # Static Assets (favicon, manifest, index.html)
├── src/
│   ├── assets/                 # Logo, hình ảnh, icon, font dùng chung
│   ├── components/             # Components UI dùng chung toàn app (Button, Input, Modal, Table)
│   ├── constants/              # Biến hằng số (AppConfig, Roles, Endpoints)[cite: 1, 3]
│   ├── context/ / store/       # Global State Management (Zustand, Redux Toolkit, Context API)[cite: 4, 6]
│   ├── hooks/                  # Custom Hooks dùng chung (useDebounce, useLocalStorage, useMediaQuery)
│   ├── layouts/                # Cấu trúc khung trang (MainLayout, AuthLayout, AdminLayout)
│   ├── routes/                 # Định tuyến ứng dụng (AppRoutes.jsx, PrivateRoute.jsx)
│   ├── services/ / api/        # Cấu hình Axios Client, Interceptors, Base API[cite: 4, 6]
│   ├── utils/                  # Hàm tiện ích (formatDate, formatCurrency, validators)
│   │
│   ├── modules/ / features/    # 🎯 TRỌNG TÂM: Chia theo từng TÍNH NĂNG NGHIỆP VỤ
│   │   ├── auth/               # Feature: Đăng nhập / Đăng ký[cite: 1, 4]
│   │   │   ├── api/            # API call riêng cho Auth (loginApi.js)
│   │   │   ├── components/     # Component nội bộ của Auth (LoginForm.jsx)
│   │   │   ├── hooks/          # Custom Hooks riêng (useAuth.js)[cite: 1, 2]
│   │   │   └── pages/          # Trang màn hình (LoginPage.jsx, RegisterPage.jsx)
│   │   │
│   │   ├── tour-booking/       # Feature: Tìm kiếm & Đặt Tour[cite: 1, 4]
│   │   │   ├── api/            # tourBookingApi.js[cite: 2, 4]
│   │   │   ├── components/     # TourCard.jsx, TourFilter.jsx[cite: 2, 5]
│   │   │   └── pages/          # TourSearchPage.jsx, TourDetailPage.jsx[cite: 2, 5]
│   │   │
│   │   ├── audio-guidance/     # Feature: Thuyết minh tự động[cite: 1, 4]
│   │   │   ├── api/            # audioApi.js[cite: 2, 4]
│   │   │   ├── components/     # AudioPlayerBar.jsx, TranscriptViewer.jsx[cite: 2, 4]
│   │   │   └── pages/          # AudioGuidePage.jsx[cite: 2]
│   │   │
│   │   └── admin-dashboard/    # Feature: Quản trị Admin[cite: 1, 4]
│   │       ├── components/     # PoiDataTable.jsx, MediaUploader.jsx[cite: 2, 4]
│   │       └── pages/          # PoiManagementPage.jsx[cite: 2]
│   │
│   ├── App.jsx                 # Root Component
│   ├── main.jsx (hoặc index.js)# Entry point ứng dụng
│   └── index.css / App.css     # Global Styles (Tailwind CSS, CSS Variables)
├── .env                        # Biến môi trường (VITE_API_BASE_URL)
├── package.json
└── README.md
