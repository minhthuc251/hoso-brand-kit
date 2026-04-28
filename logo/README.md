# Logo Assets

Bộ logo HOSO — vector tracing từ raster cũ + normalize về brand palette chuẩn.

> **Lưu ý nguồn gốc:** v0.1 các SVG được vector-trace từ PNG raster vì file source `.ai` gốc không tìm thấy. Chất lượng tốt cho mọi use case digital + in offset thông thường. Nếu sau này tìm được file `.ai` master, mở PR replace để có quality "studio" tuyệt đối.

## Cấu trúc

```
logo/
├── primary/                          # Logo chính — dùng mặc định
│   ├── horizontal.svg / .png         # Icon + chữ HOSO ngang (786×250)
│   └── vertical.svg / .png           # Icon trên + chữ dưới (600×600 square)
│
├── logomark/                         # Chỉ icon (túi giấy + lá xanh + chữ H)
│   └── logomark.svg / .png           # 281×318
│
├── wordmark/                         # Chỉ chữ "HOSO"
│   └── wordmark.svg / .png           # 786×250
│
├── monochrome/                       # Phiên bản đơn sắc
│   ├── black.svg                     # Logomark đen (chữ H trắng knockout) — dùng trên nền sáng
│   ├── white.svg                     # Logomark trắng (chữ H transparent) — dùng trên nền tối / ảnh
│   ├── single-color-green.svg        # Logomark 1 màu xanh primary — dùng khi in 1 màu
│   ├── black-horizontal.svg          # Horizontal đen — favicon đen, dấu nước
│   └── white-horizontal.svg          # Horizontal trắng — overlay trên ảnh
│
└── favicon/
    ├── favicon.ico                   # 16/32/48px — browser tab
    ├── favicon.svg                   # SVG vector — browser modern
    └── apple-touch-icon.png          # 180×180 — iOS home screen
```

## Quy tắc dùng

### ✅ NÊN
- Dùng `primary/horizontal.svg` cho mọi context có chiều ngang đủ rộng (header, email signature, business card)
- Dùng `primary/vertical.svg` khi không gian vuông/dọc (hộp sản phẩm, label, post Instagram)
- Dùng `logomark/logomark.svg` khi đã có chữ "HOSO" gần đó hoặc không gian rất nhỏ (favicon, app icon, watermark)
- Dùng `monochrome/black.svg` trên nền màu sáng/trắng/giấy kraft
- Dùng `monochrome/white.svg` trên nền tối/ảnh chụp
- Dùng `monochrome/single-color-green.svg` khi in 1-color cost-effective (khắc dấu, in lưới đơn giản)
- Giữ tối thiểu 16px clear space xung quanh logo (đo bằng chiều cao chữ "H")
- Logo tối thiểu: horizontal 80px width, logomark 24px, favicon 16px

### ❌ KHÔNG NÊN
- Không thay đổi tỉ lệ logo (stretch/skew)
- Không thay đổi màu logo ngoài 4 brand colors (xem `tokens/colors.json`)
- Không thêm shadow / glow / outline / 3D effect
- Không xoay logo trừ trường hợp watermark mờ
- Không đặt logo trên nền có pattern phức tạp — dùng white.svg hoặc bg overlay trắng/đen
- Không tự tạo phiên bản mới — mở PR đề xuất nếu cần

## Re-build logo từ source PNG

Nếu bạn có file PNG mới chất lượng cao hơn, có thể re-trace bằng:

```bash
pip install --user vtracer cairosvg pillow
# Sau đó chạy script trong scripts/build-logo.py (sẽ thêm trong PR sau)
```

## Phiên bản tương lai

Khi có file `.ai`/`.fig` master, replace tất cả SVG bằng export trực tiếp từ source. Mở PR với label `logo-master` để track.
