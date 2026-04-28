# HOSO Brand Kit

> Bộ nhận diện thương hiệu **HOSO** (Công ty TNHH giải pháp bao bì HOSO) — thiết kế AI-friendly, machine-readable.

**Slogan:** *Đồng hành kinh doanh — Nâng tầm thương hiệu*
**Hotline:** `0348 989 949` · **Website:** [tuigiayhoso.com](https://tuigiayhoso.com)

---

## Đây là gì?

Repo này là **single source of truth** cho mọi yếu tố nhận diện HOSO: logo, màu, font, voice, photography style, prompt template AI, content template, và các module riêng cho từng ngành hàng.

Repo được thiết kế **hybrid** — vừa là Git repo (versioning, PR review, public access cho freelancer/agency), vừa là **Claude skill** (auto-trigger trong Claude Code/Desktop khi nhắc HOSO).

## Cách dùng — chọn theo vai trò của bạn

### 1. Bạn dùng Claude Code / Claude Desktop

```bash
git clone https://github.com/minhthuc251/hoso-brand-kit.git ~/.claude/skills/hoso-brand
```

Xong — Claude tự trigger skill khi bạn nhắc HOSO ("viết caption FB cho HOSO", "tạo prompt ảnh sản phẩm HOSO"...).

### 2. Bạn dùng ChatGPT / Gemini / AI khác

Copy nội dung [`ai-prompts/system-prompt-hoso-assistant.md`](ai-prompts/system-prompt-hoso-assistant.md) → paste làm Custom GPT instruction (ChatGPT Plus) hoặc System Prompt (API). Xong — AI viết content đúng giọng HOSO.

> File này có sau Phase 5 của roadmap. Hiện đang scaffold.

### 3. Bạn là designer / freelancer / agency

- Logo: tải từ [`logo/`](logo/) (SVG, PNG, các phiên bản)
- Màu: [`tokens/colors.json`](tokens/colors.json)
- Font: xem [`tokens/typography.json`](tokens/typography.json) (Lexend Deca + Bricolage Grotesque, free Google Fonts)
- Voice + content guideline: [`voice/voice-guide.md`](voice/voice-guide.md)

### 4. Bạn dùng Midjourney / Imagen / Sora

Mở [`visuals/prompt-templates/`](visuals/prompt-templates/) → pick template phù hợp → copy prompt → paste vào tool image-gen.

---

## Trạng thái hiện tại

🚧 **v0.0.1-scaffold** — đang ở Phase 0. Cấu trúc đã setup, content sẽ được build qua 6 phase đến v1.0 (xem [`BRAND_KIT_DECISIONS.md`](BRAND_KIT_DECISIONS.md) section 13).

---

## Cấu trúc repo

```
.
├── SKILL.md                          # Claude skill orchestrator
├── README.md                         # File này
├── BRAND_KIT_DECISIONS.md            # 14 quyết định gốc — single source of truth
├── CHANGELOG.md
├── LICENSE                           # CC BY 4.0 cho docs
├── tokens/                           # Design tokens (JSON, CSS)
├── logo/                             # Asset logo
├── voice/                            # Brand voice guide + content templates
├── visuals/                          # Photography style + AI prompt templates + illustration
├── industries/                       # Module riêng cho 6 ngành ưu tiên
├── ai-prompts/                       # Master system prompt cho non-Claude AI
├── social/                           # Template post FB/IG/Tiktok
├── stationary/                       # Card visit, envelope, folder, apparel
└── archive/                          # Brand guideline cũ (PDF)
```

---

## License

- **Documentation, voice guide, content templates:** [CC BY 4.0](LICENSE) — cho phép dùng + sửa, phải credit
- **Logo, photography, illustration assets:** **CC BY-NC-ND 4.0** — cho phép xem/dùng tham khảo, không thương mại, không sửa, phải credit. Asset chỉ được sử dụng thương mại bởi HOSO và đối tác được ủy quyền.

Xem chi tiết trong [LICENSE](LICENSE).

---

## Đóng góp

| Cấp | Quyền |
|---|---|
| Owner (@minhthuc251) | Approve mọi thay đổi cấp brand (logo, palette, archetype, voice fundamentals) |
| Maintainer | Push trực tiếp các thay đổi nhỏ (vocab, prompt template, ví dụ) |
| Contributor | Mở PR, không push trực tiếp `main` |

Bất cứ ai (kể cả AI agent) đều có thể đóng góp qua PR. Mọi PR cần ít nhất 1 review trước khi merge.

---

🌱 *Made with care by HOSO. Đồng hành kinh doanh — Nâng tầm thương hiệu.*
