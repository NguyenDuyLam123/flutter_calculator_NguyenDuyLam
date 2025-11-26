flutter_advanced_calculator_NguyenDuyLam
Advanced Scientific & Programmer Calculator (Flutter)

* Một ứng dụng máy tính nâng cao hỗ trợ:

    - Basic Mode

    - Scientific Mode

    - Programmer Mode

    - History

    - Memory Registers

    - Settings (Angle Mode, Precision, Theme)

    - Persistent Storage (SharedPreferences)

* Features
    - Basic Mode

        + Cộng, trừ, nhân, chia

        + CE, C, %, ±

        + Memory: MC, MR, M+, M-

    - Scientific Mode

        + sin, cos, tan

        + ln, log

        + √, x², xʸ

        + π

        + DEG ⇄ RAD

        + Hỗ trợ implicit multiply: 2π, 3(2+1)

    - Programmer Mode

        + Hệ đếm: BIN, OCT, DEC, HEX

        + Toán tử: AND, OR, XOR

        + Shift: <<, >>

        + Chuyển đổi qua lại giữa các hệ đếm

    - History

        + Lưu danh sách phép tính cũ

        + Chọn lại phép tính từ lịch sử

        + Giới hạn số lượng (cài trong Settings)

    - Settings

        + Angle mode: DEG / RAD

        + Precision: 2–10

        + Theme: Light / Dark / System

        + Clear history

        + Tự động lưu bằng SharedPreferences

    - UI

        + Responsive

        + Hỗ trợ Dark Mode

        + Animation nhẹ

* Screenshots

(Save vào thư mục screenshots/)

Basic           Scientific          Programmer
basic.png	    scientific.png	    programmer.png

Settings        History
settings.png	history.png

* Architecture Diagram

lib/
 ├── providers/
 │    ├── calculator_provider.dart
 │    └── theme_provider.dart
 ├── services/
 │    └── storage_service.dart
 ├── utils/
 │    └── expression_parser.dart
 ├── screens/
 │    ├── calculator_screen.dart
 │    ├── settings_screen.dart
 │    └── history_screen.dart
 └── widgets/
      ├── button_grid.dart
      └── display_area.dart

* Setup Instructions
    1. Clone project
        git clone https://github.com/NguyenDuyLam123/flutter_advanced_calculator_NguyenDuyLam.git

    2. Install packages
        flutter pub get

    3. Run project
        flutter run

* Testing Instructions
    - Chạy tất cả test:
        + flutter test


    - Output kỳ vọng:

        + All parser tests passed

        + All programmer mode tests passed

        + Coverage > 80%

* Known Limitations

    - Chưa hỗ trợ biểu thức quá dài (>100 ký tự)

    - Chưa có voice input

    - Chưa có biểu đồ hàm số (graph plot)

* Future Improvements

    - Export history to CSV / PDF

    - Custom theme builder

    - Support for tablet & landscape mode

    - Offline syncing