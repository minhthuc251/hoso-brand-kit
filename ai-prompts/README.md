# Biến brand kit thành công cụ marketing dùng mỗi ngày

> Mục tiêu: mỗi marketer chỉ cần **1 cú click mở link**, gõ brief, nhận caption/email/mô tả **đúng giọng HOSO trong 10 giây** — không cần git, không cần copy prompt, không cần nhớ luật.

Có 2 file trong thư mục này:
- **`system-prompt-hoso-assistant.md`** — bộ não. Là toàn bộ "luật + sự thật HOSO" đã nén để dán vào 1 trợ lý AI.
- **`facts.json`** (ở root repo) — nguồn chuẩn máy đọc được, để cập nhật khi brand đổi.

---

## Bước 1 — Dựng trợ lý dùng chung (chọn nền tảng team đang dùng)

Mở `system-prompt-hoso-assistant.md`, copy toàn bộ phần dưới dấu `───`, rồi:

### A. ChatGPT (đa số marketer) → tạo **Custom GPT**
1. ChatGPT → **Explore GPTs → Create → Configure**.
2. Dán khối vừa copy vào ô **Instructions**. Đặt tên "HOSO Content Assistant", ảnh = logo.
3. (Nên) đính kèm `facts.json` vào **Knowledge** để nó tra fact chuẩn.
4. **Save → Chỉ những người có link** → copy link, gửi cả phòng.
> Cần tài khoản ChatGPT có quyền tạo GPT (Plus/Team/Enterprise). Team plan là hợp lý nhất để chia sẻ.

### B. Gemini → tạo **Gem**
1. Gemini → **Gems → New Gem**.
2. Dán khối vào **Instructions**, đặt tên, (nên) upload `facts.json` làm knowledge.
3. Chia sẻ Gem cho không gian làm việc của team.

### C. Claude → tạo **Project**
1. Claude → **Projects → New Project**.
2. Dán khối vào **Custom instructions**; kéo `facts.json` + `voice/voice-guide.md` vào **Project knowledge**.
3. Chia sẻ Project với team (Team/Enterprise plan).

> **Chọn 1 là đủ để bắt đầu.** Dựng cả 3 nếu team dùng lẫn lộn — nội dung ra như nhau vì cùng 1 system prompt.

---

## Bước 2 — Cách marketer dùng hằng ngày (dán brief, không cần biết luật)

Chỉ cần mô tả tình huống, trợ lý tự áp đúng giọng + facts:

- *"Viết 3 caption FB cho persona chủ shop mới mở, sản phẩm túi kraft in logo, nhấn không ép số lượng."*
- *"Soạn email báo giá B2B cho khách mua 5.000 túi bánh trung thu, cần VAT."*
- *"Mô tả sản phẩm túi bánh mì cho landing, giọng HOSO."*
- *"Viết kịch bản TikTok 15s về cứu deadline event 2-3 ngày."*
- *"Prompt tạo ảnh sản phẩm túi kraft phong cách rustic Việt cho quán cà phê."*

Trợ lý sẽ tự: né từ cấm, dùng CTA chuẩn, gắn hashtag bắt buộc, không bịa số — và tự chạy checklist 7 điểm trước khi trả.

---

## Bước 3 — Vẫn giữ cổng người duyệt

Trợ lý chỉ ra **bản nháp**. Quy trình duyệt giữ nguyên theo `facts.json → approval_workflow`:
caption/email marketing → **Marketing lead** duyệt; báo giá B2B → **Sale lead**; blog/khủng hoảng → **Founder**. AI không tự đăng.

---

## Vì sao đây là thứ người ta MUỐN mở (không phải bị ép)

- **Nhanh hơn tự viết:** brief → caption đúng chuẩn trong 10 giây, thay vì tra voice-guide 18KB.
- **An toàn:** không sợ lỡ viết "in offset" hay "giá sốc" — trợ lý chặn sẵn.
- **Không ma sát:** 1 link, không git/markdown/CLI.
- Kit dùng để **bắt buộc TUÂN THỦ** (chuẩn), còn trợ lý này làm nó **đáng dùng** — hai thứ bổ trợ, không mâu thuẫn.

---

## Bảo trì (đừng để lệch)

`system-prompt-hoso-assistant.md` là bản **compile** từ `facts.json` + `voice/voice-guide.md`. Khi brand đổi (thêm từ cấm, đổi CTA, thêm ngành):
1. Sửa **`facts.json`** (nguồn chuẩn) qua PR.
2. Cập nhật lại system prompt cho khớp.
3. Cập nhật lại Instructions của GPT/Gem/Project (dán bản mới).

> Về dài hạn nên có script sinh `system-prompt` tự động từ `facts.json` để khỏi cập nhật tay (xem CHẶN #3 trong audit — bệnh drift). Trước mắt: 1 người (maintainer) chịu trách nhiệm đồng bộ.
