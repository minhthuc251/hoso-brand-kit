# Gói cấu hình bấm-là-xong — Trợ lý Content HOSO

> Copy các giá trị dưới đây vào Custom GPT / Gemini Gem / Claude Project. Phần **Instructions** = toàn bộ nội dung `system-prompt-hoso-assistant.md` (phần dưới dấu `───`, 7.087 ký tự — vừa giới hạn 8.000 của Custom GPT).

## Giá trị điền sẵn (dùng chung cho cả 3 nền tảng)

**Tên:** `Trợ lý Content HOSO`

**Mô tả ngắn:** `Viết caption, email, mô tả sản phẩm đúng giọng & đúng sự thật HOSO — không bịa số liệu, không sai facts chất liệu/kỹ thuật (in KTS, kraft nguyên sinh); MOQ/lead time cụ thể thì hỏi người phụ trách, không đoán.`

**Instructions:** dán toàn bộ phần paste-được trong `ai-prompts/system-prompt-hoso-assistant.md`.

**Câu gợi ý mở đầu (conversation starters — copy 4 dòng):**
- `Viết 3 caption Facebook cho [sản phẩm] — persona chủ shop nhỏ mới mở.`
- `Soạn email báo giá B2B cho khách mua [số lượng] [sản phẩm], cần VAT.`
- `Viết mô tả sản phẩm cho trang landing: [sản phẩm].`
- `Gợi ý prompt tạo ảnh sản phẩm [sản phẩm] phong cách rustic Việt.`

**File nạp làm Knowledge (upload để trợ lý tra fact chuẩn, chống bịa):**
1. `facts.json` ← quan trọng nhất
2. `voice/voice-guide.md`
3. `voice/examples-good.md` + `voice/examples-bad.md`
4. `voice/content-templates/*.md`

---

## A. ChatGPT — Custom GPT
1. **Explore GPTs → Create → Configure**.
2. **Name / Description / Instructions / Conversation starters** ← dán từ khối trên.
3. **Knowledge → Upload files** ← 4 nhóm file ở trên.
4. **Capabilities:** bật *Web Search* nếu muốn tra xu hướng; TẮT nếu muốn trợ lý chỉ bám facts (an toàn hơn, chống bịa). Khuyến nghị: TẮT lúc đầu.
5. **Save → "Anyone with the link"** → copy link, gửi cả phòng marketing.
> Cần gói ChatGPT tạo được GPT (Plus/Team/Enterprise). **Team** là hợp lý nhất để chia sẻ nội bộ.

## B. Gemini — Gem
1. **Gems → New Gem**.
2. **Name / Instructions** ← dán. Upload `facts.json` (+ voice-guide) làm knowledge.
3. Lưu → chia sẻ Gem cho không gian làm việc của team.

## C. Claude — Project
1. **Projects → New Project**.
2. **Custom instructions** ← dán. Kéo `facts.json` + `voice/voice-guide.md` + `content-templates/` vào **Project knowledge**.
3. Chia sẻ Project với team (Team/Enterprise).

---

## Bảng "gõ gì mỗi ngày" (dán cho marketer)

| Cần gì | Gõ |
|---|---|
| Caption FB/IG | *"Viết 3 caption FB cho [SP], persona [chủ shop/event/B2B], nhấn [ý chính]."* |
| Email báo giá | *"Email báo giá cho khách mua [SL] [SP], cần VAT, giọng HOSO."* |
| Mô tả SP | *"Mô tả [SP] cho landing/Shopee, giọng HOSO."* |
| Kịch bản TikTok | *"Kịch bản TikTok 15s về [chủ đề], nhấn cứu deadline 2-3 ngày."* |
| Prompt tạo ảnh | *"Prompt ảnh sản phẩm [SP] phong cách rustic Việt cho [ngành]."* |
| Nội dung dịp lễ | *"Caption Trung Thu cho khách [ngành], không tạo urgency giả."* |

**Luôn nhớ:** trợ lý ra **bản nháp** → người duyệt trước khi đăng (theo `facts.json › approval_workflow`).

---

## Bảo trì (1 người maintainer)
Khi brand đổi (thêm từ cấm, đổi CTA, thêm ngành): sửa `facts.json` (nguồn chuẩn) → cập nhật `system-prompt-hoso-assistant.md` → dán lại Instructions của GPT/Gem/Project. *(Về dài hạn: script sinh system-prompt tự động từ facts.json — xem CHẶN #3 audit.)*
