# HOSO Video Guide

Quy tắc bắt buộc khi dựng **mọi** video HOSO: Reel, video post fanpage, TikTok, video sản phẩm.

> **Thứ tự ưu tiên khi có mâu thuẫn:** `facts.json` → `SKILL.md` → file này → thẩm mỹ của người dựng.
> Video là dạng nội dung dễ vi phạm nhận diện nhất, vì công cụ dựng (và AI) luôn có màu, font, easing mặc định của riêng chúng. Mặc định của công cụ **không bao giờ** thắng token của HOSO.

## 1. Nội dung — điều gì bắt buộc phải có

Mỗi video phải có đủ:

1. **Ít nhất một cảnh chứng minh vật liệu.** Cận cảnh thớ giấy, mép giấy, quai xoắn, hoặc mực thấm vào giấy. Nói "giấy tốt" trên hình túi chụp xa là nói suông.
2. **CTA lấy từ thư viện `SKILL.md`, không tự chế.** Và CTA **phải nhắc gửi mẫu miễn phí / in test miễn phí** — đây là selling point đặc biệt của HOSO.
3. **End card** ≥ 2.5 giây: logo + hotline `0348 989 949` + `tuigiayhoso.com`.

Nên có khi hợp ngữ cảnh: slogan *"Đồng hành kinh doanh — Nâng tầm thương hiệu"*, và **in phun kỹ thuật số** (selling point, không phải hạn chế).

Khi nói về "xanh", phải nói **cả hai tầng** (xem `facts.json › green_packaging`): tầng vật lý (kraft nguyên sinh, mực gốc nước, quai xoắn giấy) **và** tầng dòng tiền (MOQ linh hoạt nên không ôm kho, 2-3 ngày nên không phải đặt sớm rồi lỗi mốt).

## 2. Lời thoại và chữ trên màn hình

`vocab.blocklist` áp dụng cho **cả lời đọc lẫn chữ hiển thị** — không chỉ caption. Riêng với video, chú ý:

- Không hứa vượt `facts.json`. Sai lead time và sai MOQ là lỗi hay gặp nhất; tra bảng `vocab.product_error_corrections` trước khi viết.
- Không bịa số liệu ("300+ thương hiệu đã tin dùng") — xem `facts.json › no_fabrication_rule`.
- Xưng hô "HOSO" – "bạn".
- Đọc số điện thoại theo đúng nhóm `0348 989 949`. Ghi sai nhóm thì giọng AI cũng đọc sai.

## 3. Màu

Chỉ dùng token trong `tokens/colors.json`.

| Vai trò trong video | Token |
|---|---|
| Nhấn, CTA, gạch chân, viền active | `brand.primary` `#78bc20` |
| Nền tối, footer, chữ trên nền sáng | `neutral.dark` `#603a17` |
| Nền sáng, card, khối chữ | `neutral.light` `#f4e6d7` |
| Chữ body | `neutral.black` `#1a1a1a` |

**Vàng/gold không phải màu HOSO.** Brand cũ có vàng; bộ nhận diện hiện tại thì không. Không dùng vàng làm màu nhấn, kể cả cho số liệu hay badge.

**Không dùng `#000000`** — kể cả cho nền hộp phụ đề. Dùng `#1a1a1a`.

Với cảnh quay/ảnh thật, theo `facts.json › photography.grading`: warm 3200–4500K, saturation vừa, contrast mềm. Màu xanh `#78bc20` **đến từ sản phẩm trong khung hình, không phủ overlay xanh lên ảnh**. Xanh chỉ dùng làm màu đồ họa ở lớp chữ/khối, không phải lớp ảnh.

## 4. Chữ

Theo `tokens/typography.json`: heading **Bricolage Grotesque**, body **Lexend Deca**, trích dẫn **Lora**, số liệu/mã túi **JetBrains Mono**. Cả bốn đều là Google Fonts miễn phí và đủ dấu tiếng Việt.

Quy tắc riêng cho video, cộng thêm quy tắc chung trong token:

- Tối đa **2 weight** trong một video.
- **Không quá 4 từ in hoa liên tiếp** (trừ wordmark). Câu khẩu hiệu dài phải viết thường.
- Heading tracking `-0.02em`, line-height 1.1–1.3.
- Cỡ chữ nhỏ nhất **44px** ở khung rộng 1080. Chữ trên video bị nén và xem trên điện thoại — nhỏ hơn là mất chữ.
- Chữ không italic, trừ trích dẫn và tên sản phẩm.

## 5. Bố cục — vùng an toàn

Xem `tokens/motion.json › safeArea`. Với Reel, UI Facebook che **12% trên, 22% dưới, 14% phải**. Chữ hoặc logo đặt ngoài vùng này sẽ bị caption và cột nút che mất. Đây là lỗi phổ biến nhất khi đăng Reel và chỉ phát hiện được sau khi đã đăng.

## 6. Chuyển động

Easing chủ đạo là `motion.easing.press` — vào nhanh, dừng dứt khoát, lắng nhẹ, mô phỏng **con dấu chạm mặt giấy**. Ngôn ngữ chuyển động của HOSO bắt nguồn từ chính hành vi in ấn lên giấy, nên nó vừa riêng vừa đúng nghề.

Cấm chuyển động trôi lững lờ (chữ bay lên rồi mờ dần — mặc định của mọi template AI). Ảnh tĩnh phải có camera, nhưng zoom tối đa 1.18× và luôn giảm tốc, không trôi đều hai chiều.

Cảnh ngắn nhất 1.6 giây. Ngắn hơn thì người xem không kịp đọc.

## 7. Logo

Luôn dùng file trong `logo/` — SVG cho mọi khâu dựng. **Không bao giờ** tách logo ra khỏi ảnh chụp bằng color key: viền sẽ bẩn và phóng to sẽ rỗ.

Không đổi màu logo, không kéo méo, không tách rời phần biểu tượng khỏi chữ, không thêm đổ bóng lên logo. Trên nền tối dùng `logo/monochrome/white.svg`; nền sáng dùng `logo/primary/`.

## 8. Phụ đề

Phần lớn người xem Reel tắt tiếng. Phụ đề là **bắt buộc**, trừ một trường hợp: chữ động đã mang trọn vẹn lời thoại. Khi đó **không** thêm phụ đề nữa — chữ đôi cùng nội dung trông nghiệp dư.

Thông số ở `tokens/motion.json › subtitle`.

## 9. Cấm khi dựng và khi quay

Kế thừa toàn bộ `facts.json › photography.forbidden`, và với video còn thêm:

- Nhựa, túi nylon, hộp xốp — kể cả nằm mờ trong hậu cảnh.
- Pastel teen (hồng phấn, lavender, mint).
- Người mẫu Tây phương rõ nét.
- Nhạc có lời tiếng Anh át lời thoại tiếng Việt.
- Footage stock nước ngoài đóng vai sản phẩm HOSO.
- AI sinh chữ hoặc sinh logo trong khung hình — chữ và logo phải overlay sau bằng file thật.

## 10. Checklist trước khi đăng

- [ ] Mọi con số đối chiếu khớp `facts.json` (lead time, MOQ, vật liệu, kiểu in)
- [ ] Không có từ nào trong `vocab.blocklist`, kể cả chữ trên màn hình
- [ ] CTA lấy từ thư viện và có nhắc mẫu miễn phí / in test miễn phí
- [ ] Màu chỉ nằm trong `tokens/colors.json`; không có vàng; không có `#000000`
- [ ] Font đúng Bricolage Grotesque / Lexend Deca; không quá 2 weight; không quá 4 từ in hoa liên tiếp
- [ ] Chữ và logo nằm trong vùng an toàn của nền tảng
- [ ] Có ít nhất một cảnh chứng minh vật liệu
- [ ] End card ≥ 2.5s, hotline viết đúng `0348 989 949`
- [ ] Logo dùng từ `logo/`, không color key, không đổi màu
- [ ] Phụ đề có, hoặc chữ động đã thay thế trọn vẹn — không có cả hai

---

**Source of truth:** github.com/minhthuc251/hoso-brand-kit
