# HOSO Brand Kit — Hướng dẫn dùng cho nhân sự

> Bộ "não thương hiệu" của **HOSO** (Công ty TNHH giải pháp bao bì HOSO). Cắm vào AI (ChatGPT/Gemini/Claude) để viết caption, email, mô tả sản phẩm **đúng giọng HOSO và đúng sự thật** — không bịa, không sai facts.

**Slogan:** *Đồng hành kinh doanh — Nâng tầm thương hiệu* · **Hotline:** `0348 989 949` · **Website:** [tuigiayhoso.com](https://tuigiayhoso.com)

---

## Bộ này giúp bạn gì?

Bạn gõ một câu brief ("viết 3 caption FB cho quán cà phê mới") → AI trả về content **đã đúng giọng HOSO, đúng facts, đủ hashtag, né từ cấm** — trong ~10 giây. Bạn không cần thuộc lòng voice guide; kit lo phần đó.

## ⚡ Bắt đầu nhanh nhất (marketer)

Đội đã dựng sẵn **1 trợ lý dùng chung** (Custom GPT / Gemini Gem / Claude Project).

- **Đã có link trợ lý?** → mở link, gõ brief, xong. Kéo xuống mục [Dùng mỗi ngày](#dùng-mỗi-ngày).
- **Chưa có, cần dựng?** → làm theo **[`ai-prompts/setup-pack.md`](ai-prompts/setup-pack.md)** (có sẵn tên, mô tả, câu gợi ý, file cần nạp — chỉ việc copy-dán, ~10 phút, làm 1 lần cho cả phòng).

## Chọn cách dùng theo vai trò

### 1. Bạn dùng ChatGPT / Gemini (đa số marketer)
Dùng trợ lý dùng chung ở trên. Chưa có link thì tự dựng theo [`ai-prompts/setup-pack.md`](ai-prompts/setup-pack.md).

### 2. Bạn muốn thử NGAY, không dựng gì (30 giây)
Mở [`ai-prompts/system-prompt-hoso-assistant.md`](ai-prompts/system-prompt-hoso-assistant.md), copy phần **giữa 2 dấu `───`**, dán làm **tin nhắn đầu tiên** trong bất kỳ chat AI nào, rồi gõ brief bên dưới. Dùng liền — chỉ là không lưu lại cho lần sau.

### 3. Bạn dùng Claude Code / Claude Desktop
```bash
git clone https://github.com/minhthuc251/hoso-brand-kit.git ~/.claude/skills/hoso-brand
```
Xong — Claude tự bật skill khi bạn nhắc "HOSO / viết caption HOSO / túi kraft". Cập nhật sau: `git -C ~/.claude/skills/hoso-brand pull`.

### 4. Bạn là designer / freelancer
- Logo: [`logo/`](logo/) (SVG + PNG, đủ biến thể)
- Màu / font / spacing: [`tokens/`](tokens/) — `colors.json`, `typography.json`, `tokens.css` (import thẳng vào Figma / CSS)
- Giọng + ví dụ: [`voice/`](voice/)

### 5. Bạn cần prompt tạo ẢNH
Hỏi thẳng trợ lý (đường 1): *"Prompt tạo ảnh túi kraft phong cách rustic Việt cho tiệm bánh."* Trợ lý lấy phong cách/điều-cấm từ `facts.json`. *(Thư viện prompt ảnh sẵn `visuals/` đang trong roadmap.)*

---

## Dùng mỗi ngày

Gõ brief tự nhiên, không cần biết luật:

| Cần gì | Gõ |
|---|---|
| Caption FB/IG | *"Viết 3 caption FB cho [SP], persona [chủ shop/event/B2B], nhấn [ý chính]."* |
| Email báo giá | *"Email báo giá cho khách mua [SL] [SP], cần VAT, giọng HOSO."* |
| Mô tả SP | *"Mô tả [SP] cho landing/Shopee, giọng HOSO."* |
| Kịch bản TikTok | *"Kịch bản TikTok 15s về [chủ đề], nhấn cứu deadline 2-3 ngày."* |
| Nội dung dịp lễ | *"Caption Trung Thu cho khách [ngành], không tạo urgency giả."* |

## 🔒 Hai quy tắc vàng (bắt buộc)

1. **AI ra BẢN NHÁP — người duyệt trước khi đăng.** Ai duyệt gì xem [`facts.json`](facts.json) mục `approval_workflow` (caption → Marketing lead; báo giá → Sale lead; blog/khủng hoảng → Founder).
2. **Không đăng số liệu/tên đối tác mà kit không có.** Trợ lý được lập trình để không bịa; nếu bạn tự thêm số, phải là số thật.

---

## Có gì trong kit

**✅ Dùng được ngay**
- [`facts.json`](facts.json) — nguồn sự thật máy đọc (facts SP, 4 core value, 4 hàng rào, persona, vocab, CTA, màu, checklist)
- [`ai-prompts/`](ai-prompts/) — system prompt + hướng dẫn dựng trợ lý ([`setup-pack.md`](ai-prompts/setup-pack.md))
- [`voice/`](voice/) — voice guide + ví dụ đúng/sai + template FB/email/landing/product
- [`tokens/`](tokens/) · [`logo/`](logo/) — màu, font, logo
- [`SKILL.md`](SKILL.md) — bản cho Claude Code

**🚧 Đang trong roadmap (chưa có)**
- `industries/` (module 6 ngành) · `visuals/` (thư viện prompt ảnh + ref) · `social/` · `stationary/`

*(Xem [`BRAND_KIT_DECISIONS.md`](BRAND_KIT_DECISIONS.md) cho toàn bộ quyết định gốc.)*

---

## License & đóng góp

- **Docs / voice / content:** [CC BY 4.0](LICENSE) — dùng + sửa, phải credit.
- **Logo / ảnh / illustration:** CC BY-NC-ND 4.0 — không thương mại, không sửa; chỉ HOSO & đối tác được ủy quyền dùng thương mại.

| Cấp | Quyền |
|---|---|
| Owner (@minhthuc251) | Duyệt thay đổi cấp brand (logo, màu, archetype, voice, **core value / hàng rào**) |
| Maintainer | Push thay đổi nhỏ (vocab, template, ví dụ) |
| Contributor | Mở PR, không push thẳng `main`; mỗi PR cần ≥1 review |

> **Sửa brand thì sửa ở đâu?** Voice/màu/giá trị → sửa `facts.json` + `voice-guide.md` (đây là nhà chính), rồi cập nhật lại Instructions của trợ lý. **Thông tin per-sản-phẩm và tệp khách hàng KHÔNG nằm ở đây** — cái đó sống trong ERP, AI lấy qua MCP.

---

🌱 *Made with care by HOSO. Đồng hành kinh doanh — Nâng tầm thương hiệu.*
