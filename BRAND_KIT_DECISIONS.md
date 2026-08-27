# HOSO Brand Kit — Decisions v1.0

> Tổng hợp 14 quyết định brand identity cho HOSO, output của session grill-me ngày 2026-04-28.
> File này là **single source of truth** cho execution roadmap. Mọi file/asset tạo sau này phải khớp với decisions ở đây.

---

## 0. Context & Mục tiêu

**Brand:** Công ty TNHH giải pháp bao bì HOSO
**Slogan:** "Đồng hành kinh doanh — Nâng tầm thương hiệu"
**Hotline:** `0348 989 949`
**Mục tiêu brand kit mới:** AI-friendly, machine-readable, đáp ứng việc dùng AI để (B) viết content, (A) generate ảnh marketing, (C) tạo document/slide, (D) build web/app.

**Ưu tiên use case:** **B → A → C → D**

---

## 1. Brand Archetype

- **Primary: Caregiver** — đồng hành, chu đáo, "chúng tôi lo cho bạn"
- **Secondary: Creator** — đam mê thiết kế, kể câu chuyện, nâng tầm thương hiệu khách
- **Bỏ:** Everyman (mâu thuẫn với "nâng tầm")

**Tại sao:** Slogan có 2 vế khớp đúng 2 archetype này. Khách B2B mua bao bì = mua sự yên tâm + cảm giác được nâng cấp.

---

## 2. Color Palette

### Base (6 role)

```json
{
  "primary":       { "hex": "#78bc20", "rgb": "120,188,32", "cmyk": "58,2,100,0",  "role": "logo, CTA chính" },
  "primary-dark":  { "hex": "#519600", "rgb": "81,150,0",   "cmyk": "73,19,100,4", "role": "hover, accent, footer" },
  "neutral-dark":  { "hex": "#603a17", "role": "text trên nền sáng, vibe organic" },
  "neutral-light": { "hex": "#f4e6d7", "role": "nền section, cảm giác giấy kraft" },
  "white":         { "hex": "#ffffff", "role": "nền chính" },
  "black":         { "hex": "#1a1a1a", "role": "text body — KHÔNG dùng đen tuyền #000" }
}
```

### Semantic (4)

```json
{
  "success": "#519600",
  "warning": "#e8a317",
  "error":   "#c0392b",
  "info":    "#3b7ea8"
}
```

**Quan trọng:** PDF cũ ghi "Color of brand: Vàng" — **SAI**. Primary thực sự là xanh lá `#78bc20`. Phải sửa ở mọi văn bản kế thừa.

---

## 3. Voice — Tone Attributes

| Spectrum | Vị trí HOSO |
|---|---|
| Funny ↔ Serious | **Serious 55%** (hơi nghiêng giữa) |
| Formal ↔ Casual | **Casual 60%** |
| Respectful ↔ Irreverent | **Respectful 100%** (tuyệt đối) |
| Enthusiastic ↔ Matter-of-fact | **Enthusiastic 60%** |

### Xưng hô

- **Default (90%):** "HOSO" – "bạn"
- **Formal (hợp đồng, báo giá enterprise):** "HOSO" – "Quý khách"
- **Cấm:** "shop", "ad", "mình ơi", "iu", "chúng mình"

---

## 4. Vocab Lists

### Khuyến khích (allowlist)
- **Đồng hành (Caregiver):** đồng hành, song hành, cùng bạn, hỗ trợ, lắng nghe, tư vấn, chu đáo, tận tâm
- **Nâng tầm (Creator):** nâng tầm, kể câu chuyện, thiết kế, tinh chỉnh, ấp ủ, chăm chút từng chi tiết, form, chất cảm
- **Bền vững:** bao bì xanh, thân thiện môi trường, giấy kraft, tái chế, bền vững, có trách nhiệm
- **Chuyên nghiệp:** đúng hẹn, đúng spec, kiểm soát chất lượng, lead time, MOQ, mẫu in thử
- **Free sample (selling point):** gửi mẫu miễn phí, in test miễn phí, xem hàng thực tế trước khi đặt

### Cấm tuyệt đối (blocklist)
- **Tiếng lóng/teen:** đỉnh, đỉnh chóp, xỉu, mê li, iu, hong, ko, gòi, nha, nhe, nè
- **Sale rởm:** giá sốc, rẻ vô địch, độc quyền duy nhất, số 1 không có đối thủ
- **Hype rỗng:** wow, woa, ôi, omg, cực kỳ, vô cùng tuyệt vời
- **Châm chọc đối thủ:** so với bên A/B, đối thủ chỉ là, kém HOSO, đừng dại mà chọn
- **Từ tuyệt đối:** luôn luôn, không bao giờ, 100%, mãi mãi
- **Dịch máy thô:** đáng kinh ngạc, nhân tiện, vào cuối ngày

### Linh hoạt (context-dependent)
- "khách hàng" → trang trọng OK, caption FB → "bạn"
- "chúng tôi" → hợp đồng OK, content marketing → "HOSO"
- "tuyệt vời", "đẹp" → tối đa 1 lần / bài

---

## 5. Sentence + Emoji + Hashtag + CTA Rules

### Reading level
- Câu trung bình **12–18 từ**, tối đa **25 từ**
- Đoạn tối đa **3 câu**
- Reading level lớp 9–10 (tránh Hán-Việt nặng)
- Ngôi 2 ("bạn") chủ đạo

### Emoji
- **Whitelist:** 🌱 🌿 ☘️ 📦 🎨 ✨ ✅ 📩 📞 💬
- **Blacklist:** 🤣 😂 🥰 😍 🥺 🙏(lạm dụng) ⚡ 🔥 💸 💰
- FB caption: 2–3 emoji/post; IG: 3–5; Tiktok: 3–5
- Email B2B / web / hợp đồng: **0 emoji**

### Hashtag
- Brand bắt buộc: `#HOSO #tuigiayhoso #baobixanh`
- FB: 3–5 tag; IG: 8–12; Tiktok: 4–6

### CTA library
- Tư vấn: *"Inbox HOSO để được tư vấn mẫu phù hợp — HOSO sẵn sàng gửi hàng mẫu miễn phí, thậm chí in test theo thiết kế của bạn để gửi xem trực tiếp."*
- Liên hệ: *"Gọi HOSO 0348 989 949 — sẵn sàng đồng hành cùng bạn"*
- Xem sản phẩm: *"Xem chi tiết bộ sưu tập tại tuigiayhoso.com"*

### CTA cấm
- "MUA NGAY!!!", "CHỐT ĐƠN LIỀN TAY", "INBOX NGAY KẺO LỠ"

---

## 6. Photography Style

### Phong cách chủ đạo: "Rustic Vietnam — Cuộc sống bình dân"
- **Bối cảnh:** hiên nhà gạch men, sân quê, chợ truyền thống, quán cà phê vỉa hè, mâm cơm gia đình, ban thờ ngày rằm
- **Props:** rổ tre, nón lá, gốm Bát Tràng, lụa, hoa cúc/sen/đào/mai, lá chuối, lạt buộc, đèn lồng, lì xì
- **Người:** Việt 25–60 tuổi, ưu tiên tay/lưng/chi tiết, không full face mẫu studio
- **Mood:** ấm áp, hoài niệm, "có hồn", tự hào dân tộc nhẹ

### Color grading
- Temperature: warm 3200K–4500K
- Saturation vừa, contrast mềm
- Background: kem, gỗ nhạt, vải lanh, giấy kraft
- Highlight `#78bc20` chỉ qua sản phẩm/chi tiết, không overlay

### Composition
- Rule of thirds, 30–40% negative space
- Props eco-relevant (cây xanh, gỗ, đá tự nhiên, vải lanh)
- Tránh nhựa, neon, gradient, người mẫu Tây phương rõ

### Cấm
- Nhựa, túi nylon, hộp xốp (kể cả props gián tiếp)
- Pastel teen (hồng, lavender, mint)
- AI-generated text overlay (overlay text bằng Canva sau)
- AI vẽ logo HOSO (luôn paste logo SVG vào sau)

### Lịch ngày lễ (cultural calendar)
Tết Nguyên Đán, Rằm tháng Giêng, Giỗ Tổ Hùng Vương, 30/4–1/5, Vu Lan, Trung Thu, 20/10, 8/3, 20/11, Noel & Tết Dương + tinh thần dân tộc quanh năm.

**Cấm:** Halloween, Valentine, Black Friday (trừ khi khách trong ngành đó), cờ đảng/biểu tượng nhạy cảm.

---

## 7. Industries — 6 ngành ưu tiên

| # | Ngành | Visual mood |
|---|---|---|
| 1 | F&B cà phê / trà sữa | Cà phê đang uống, vỉa hè |
| 2 | F&B bánh / dessert | Bánh + nguyên liệu, bếp gia đình |
| 3 | Thời trang local brand | Người mặc đồ cầm túi, studio mộc |
| 4 | Mỹ phẩm / skincare | Bàn vanity, hoa, đá tự nhiên |
| 5 | Thực phẩm sạch / organic | Làng quê, vườn, nắng sớm |
| 6 | **Làng nghề OCOP** ⭐ | Làng nghề, nghệ nhân, di sản |

> Cột "Sản phẩm" đã bị gỡ 27/08/2026. Nó liệt kê ly giấy, hộp bánh, hộp bánh trung thu, hộp kem, hộp giày, hộp đựng sản phẩm — HOSO không làm mặt hàng nào trong số đó. Đây là danh sách **ngành khách hàng**, không phải danh mục sản phẩm. Muốn biết HOSO làm gì: tra catalog ERP.

### Discourage list — KHÔNG chủ động chào mời (cập nhật 2026-08-24, xem mục "Lịch sử quyết định")
> Tên gốc phiên bản 2026-04-28 là "Refuse list (KHÔNG phục vụ)". Founder làm mềm 2026-08-24: đây không còn là từ chối cứng.
- Rượu, bia, đồ uống có cồn
- Đồ thủy tinh, gốm sứ giá trị cao, đồ dễ vỡ
- Đồ đông lạnh, đồ có nước/ướt
- **Lý do:** giấy không chịu nước, không đủ cứng cho đồ nặng/dễ vỡ
- **Được làm:** nếu khách các ngành trên chủ động hỏi, HOSO tư vấn thật (nói rõ giới hạn của giấy)
- **Không được làm:** chủ động pitch/chào mời HOSO cho các ngành này

---

## 8. Typography

| Role | Font | Weight | Fallback |
|---|---|---|---|
| **Heading** | **Bricolage Grotesque** | 700/800 | Inter, system-ui |
| **Body** | **Lexend Deca** | 400/500 | Inter, system-ui |
| **Body emphasis** | **Lexend Deca** | 600 | — |
| **Quote / accent** | **Lora** italic | 400 italic | Georgia |
| **Mono (giá/mã/spec)** | **JetBrains Mono** | 400 | Courier New |

### Type scale (desktop)
```
H1  48px / 1.1 / 800
H2  36px / 1.2 / 700
H3  24px / 1.3 / 700
H4  20px / 1.4 / 600
Body large 18px / 1.6 / 400
Body       16px / 1.6 / 400
Body small 14px / 1.5 / 400
Caption    12px / 1.4 / 500
```
Mobile = 80% scale (H1 → 38px, body giữ 16px).

### Rules
- Tối đa 2 weight / trang
- Heading line-height 1.1–1.3, body 1.5–1.6
- UPPERCASE max 4 từ liên tiếp (trừ wordmark)
- Body không italic (chỉ trích dẫn, tên sản phẩm)
- Heading tracking -0.02em

---

## 9. Logo Asset Convention

### Inventory: bạn có đủ file source `.ai`/`.fig` → chỉ cần export.

### Output cần có (13 file logo + favicon set)
```
logo/
├── master.ai
├── primary/{horizontal,vertical}.{svg,png}      (PNG transparent 2048px)
├── logomark/logomark.{svg,png}                  (chỉ icon)
├── wordmark/wordmark.{svg,png}                  (chỉ chữ HOSO)
├── monochrome/{black,white,single-color-green}.svg
└── favicon/{favicon.ico, favicon.svg, apple-touch-icon.png(180×180)}
```

### Approach
**100% AI-assisted** export + standardize (rotate, resize, optimize SVG, generate favicon).

---

## 10. Iconography & Illustration

### Icons
- **Bộ chính: Lucide Icons** (free MIT, ~1500 icons)
- Stroke `1.5`, sizes `16/20/24/32/48px`
- Color `currentColor` (kế thừa text color)
- AI: rút từ Lucide, **không tự generate**

### Illustration
- **80% Photo + minimal overlay** (chủ đạo)
- **20% Hand-drawn organic accent** (banner đặc biệt, key visual ngày lễ)
  - Doodle lá cây/mầm xanh
  - Pattern giấy kraft + ink stamp đỏ
  - Calligraphy thư pháp ngắn cho Tết / OCOP
  - Watercolor wash chuyển mùa

### Cấm
- Cartoon mascot kawaii/chibi
- Gradient mesh kim loại
- AI-generated nhân vật cụ thể (uncanny face)

---

## 11. Hosting & Distribution — Hybrid Repo+Skill

### Source of truth: GitHub repo `minhthuc251/hoso-brand-kit`
- **Visibility:** Public
- **License:** CC BY-NC-ND 4.0 cho asset, CC BY 4.0 cho docs
- **Branch protection:** `main` không force push, yêu cầu PR + 1 review

### Hybrid: repo cũng là Claude skill
Repo có `SKILL.md` ở root → ai clone vào `~/.claude/skills/hoso-brand` thì auto-trigger trong Claude Code/Desktop.

### Maintenance workflow
| Cấp | Người | Quyền |
|---|---|---|
| Owner | minhthuc251 | Approve thay đổi cấp brand (logo, palette, archetype, voice fundamentals) |
| Maintainer | 1–2 marketing/design lead (TBD) | Push trực tiếp thay đổi nhỏ (vocab, prompt template, ví dụ) |
| Contributor | nhân viên, freelancer, AI agent | Mở PR, không push trực tiếp |

### Versioning: SemVer
- v1.0.0 = release đầu
- v1.x.0 = thêm template/asset
- v2.0.0 = đổi lớn (logo, màu, archetype)
- `CHANGELOG.md` ghi mỗi version

### Multi-channel access
| Đối tượng | Cách dùng |
|---|---|
| Claude Code user | `git clone ... ~/.claude/skills/hoso-brand` → auto-trigger |
| ChatGPT/Gemini user | Copy `ai-prompts/system-prompt-hoso-assistant.md` → paste làm Custom GPT instruction |
| Designer/freelancer | Browse GitHub, tải `logo/`, `tokens/colors.json` qua raw URL |
| Midjourney user | Mở `visuals/prompt-templates/*.md` → copy template |
| RAG app sau này | Clone + index → vector search |

---

## 12. Repo Structure

```
hoso-brand-kit/
├── SKILL.md                                    # Skill orchestrator (~500 token)
├── README.md                                   # Human entry point
├── LICENSE
├── CHANGELOG.md
├── tokens/
│   ├── colors.json
│   ├── typography.json
│   ├── spacing.json                            # 4/8/12/16/24/32/48/64/96/128 px
│   └── tokens.css                              # CSS variables
├── logo/                                       # 13 file convention
├── voice/
│   ├── voice-guide.md
│   ├── examples-good.md                        # 30+ ví dụ "đúng giọng"
│   ├── examples-bad.md                         # 20+ ví dụ "sai giọng"
│   └── content-templates/
│       ├── facebook-caption.md
│       ├── email-marketing.md
│       ├── email-b2b-quote.md
│       ├── product-description.md
│       └── landing-hero.md
├── visuals/
│   ├── photography-style.md
│   ├── prompt-templates/
│   │   ├── product-shot.md
│   │   ├── lifestyle-cafe.md
│   │   ├── lifestyle-bakery.md
│   │   ├── lifestyle-fashion.md
│   │   ├── lifestyle-cosmetic.md
│   │   ├── lifestyle-organic.md
│   │   ├── lifestyle-ocop.md
│   │   └── seasonal-tet.md
│   ├── references/                             # 50+ ảnh curate
│   └── illustration/
│       ├── kraft-textures/
│       ├── doodle-leaves/
│       ├── stamps-seals/
│       ├── calligraphy/
│       └── patterns/
├── industries/
│   ├── fnb-cafe.md
│   ├── fnb-bakery.md
│   ├── fashion.md
│   ├── cosmetic.md
│   ├── organic-food.md
│   └── ocop-craft.md
├── ai-prompts/
│   ├── system-prompt-hoso-assistant.md         # Master cho non-Claude
│   ├── write-fb-post.md
│   ├── write-email-quote.md
│   └── generate-product-image.md
├── social/                                     # Template post FB/IG/Tiktok
│   ├── facebook/
│   ├── instagram/
│   └── tiktok/
├── stationary/                                 # Asset thừa kế PDF cũ
│   ├── card-visit/
│   ├── envelope/
│   ├── folder/
│   └── apparel/
└── archive/
    └── brand-guideline-hoso-2025.pdf
```

---

## 13. Implementation Roadmap (6 tuần đến v1.0)

| Phase | Thời gian | Output | CEO time |
|---|---|---|---|
| **0. Khởi tạo** | Ngày 1 (~2h) | Repo public, structure, README, LICENSE, branch protection, SKILL.md | ~30 phút |
| **1. Tokens + Logo** | Tuần 1 | tokens/*.json, 13 file logo + favicon set | ~1h QA |
| **2. Voice guide** ⭐ | Tuần 2 | voice-guide.md + 30 examples-good + 20 examples-bad + 5 content-template | **~3h** (CEO duyệt từng ví dụ) |
| **3. Image gen prompts** | Tuần 3 | photography-style.md + 7 prompt template + 50+ ref ảnh | ~2h pick ref |
| **4. Industry modules** | Tuần 4 | 6 file `industries/*.md`, mỗi ngành có voice variant + visual variant + 3 mẫu post + 1 case study | ~2h cung cấp khách thật |
| **5. Master AI prompts** | Tuần 5 | system-prompt-hoso-assistant.md + 4 sub-prompt | ~2h test thực tế |
| **6. Social + stationary + illustration** | Tuần 6 | 15+ social template, import stationary từ PDF, illustration accent | ~1h |
| **v1.0 release** | Tuần 6 cuối | Tag v1.0.0, CHANGELOG, announce | — |

**Tổng CEO time: ~11h trải 6 tuần (~2h/tuần).**

**100% AI-assisted** — không thuê designer ngoài cho v1.0.

---

## 14. Next Step (Bước B sau khi bạn duyệt file này)

1. Tạo public repo `minhthuc251/hoso-brand-kit` qua `gh repo create`
2. Scaffold cấu trúc thư mục Phase 0
3. Commit `v0.0.1-scaffold`
4. Setup branch protection
5. Bắt đầu Phase 1 (tokens + logo export — cần bạn share file source `.ai`/`.fig`)

---

## Lịch sử quyết định

- 2026-04-28: v1.0 — Output session grill-me. CEO @minhthuc251 chốt 14 quyết định.
- 2026-08-24: Founder chốt 2 thay đổi, phản ánh trong `facts.json` v0.4.0: (1) §7 Refuse list → Discourage list — không còn từ chối cứng, chỉ không chủ động chào mời; khách hỏi thì vẫn tư vấn thật. (2) Xác nhận HOSO dùng có chủ đích 2 kiểu xưng hô theo kênh — content một-chiều giữ "HOSO"–"bạn" (§3), chat 1-1 (chatbot web/Meta/Zalo) dùng "em"–"anh/chị" (mới, xem `facts.json › voice_channel_overrides`). Đồng thời: `product_facts` trong `facts.json` thu hẹp lại đúng phần kit sở hữu (chất liệu/kỹ thuật in) — số vận hành (MOQ, lead time, mẫu miễn phí) chuyển hẳn sang ERP `hoso_erp.business_facts`, kit chỉ giữ con trỏ (`product_facts_ref`), không giữ bản sao.
