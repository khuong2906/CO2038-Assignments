# ⏰ Digital Clock with Alarm (ATmega328P PCB Design)

[![Altium Designer](https://img.shields.io/badge/Altium_Designer-24.10+-blue.svg)](https://www.altium.com/)
[![Microcontroller](https://img.shields.io/badge/MCU-ATmega328P-red.svg)](https://www.microchip.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Dự án thiết kế bo mạch PCB cho **Đồng hồ số tích hợp báo thức (Digital Clock with Alarm)** sử dụng vi điều khiển ATmega328P, hiển thị qua 4 LED 7 đoạn và điều khiển bằng nút nhấn. Dự án nằm trong khuôn khổ bài tập lớn môn **Kỹ thuật Điện tử (EEC)** - Trường Đại học Bách Khoa, ĐHQG TP.HCM.


---

## ⚡ Tính Năng & Thông Số Kỹ Thuật

- **Vi điều khiển chính:** ATmega328P-PU (Chân PDIP-28).
- **Tần số thạch anh:** Thạch anh ngoài 16 MHz với 2 tụ xả 22pF.
- **Nguồn cấp:** Pin 9V DC, hạ áp xuống 5V DC ổn định qua IC nguồn LM7805 (kèm tụ lọc cao tần 104pF).
- **Hiển thị:** 4 LED 7 đoạn (Common Anode) quét đa hợp thể hiện Giờ - Phút.
- **Chỉ báo & Điều khiển:** 
  - 2 LED đỏ 3mm làm đèn trạng thái/báo thức (hạn dòng qua điện trở 330Ω).
  - 2 Nút nhấn (Pushbutton) cấu hình cài đặt thời gian và báo thức.
- **Thiết kế PCB:** Mạch in 2 lớp (Top Layer & Bottom Layer) phủ đồng GND cách ly chống nhiễu.

---

## 📁 Cấu Trúc Thư Mục Dự Án

```text
.
├── assignment schematic.SchDoc   # Sơ đồ nguyên lý (Schematic Design)
├── PCB1.PcbDoc                   # Sơ đồ mạch in PCB (Layout 2D & 3D Render)
├── PROJECT.PrjPcb                # File quản lý dự án Altium Designer
├── PROJECT.BomDoc                # Danh sách linh kiện (Bill of Materials)
├── PROJECT.OutJob                # File cấu hình xuất tập tin sản xuất (Gerber/Drill)
└── README.md                     # Hướng dẫn sử dụng dự án
