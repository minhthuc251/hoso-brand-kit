# Changelog

Mọi thay đổi đáng chú ý của HOSO Brand Kit đều ghi ở đây.

Format theo [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), versioning theo [SemVer](https://semver.org/).

---

## [v1.0.0] — 2026-04-28

🎉 **Release đầu tiên** — brand kit usable cho mục tiêu B (AI viết content) và D (web/dev).

### Phase 0 — Scaffold
- Repo public `minhthuc251/hoso-brand-kit` + `SKILL.md` Claude skill auto-trigger
- README + LICENSE (dual CC BY 4.0 + CC BY-NC-ND 4.0)
- `BRAND_KIT_DECISIONS.md` — 14 quyết định nền tảng từ session grill-me

### Phase 1 — Tokens + Logo
- 13 file logo (vector trace từ raster, normalize về brand palette)
  - Primary horizontal + vertical (SVG + PNG 2048px)
  - Logomark, wordmark
  - Monochrome black/white/single-color-green + horizontal variants
  - Favicon set (.ico + .svg + apple-touch-icon 180×180)
- 4 token files
  - `colors.json` — DTCG format, 6 base + 4 semantic
  - `typography.json` — Bricolage Grotesque + Lexend Deca + Lora + JetBrains Mono
  - `spacing.json` — 11-step + radius + shadow
  - `tokens.css` — CSS variables import-ready
- README cho `logo/` và `tokens/` với usage rules

### Phase 2 — Voice Guide
- `voice-guide.md` (358 dòng) — 15 sections master document
- `examples-good.md` (339 dòng) — 25+ ví dụ "đúng giọng" theo persona
- `examples-bad.md` (307 dòng) — 22 ví dụ "sai giọng" + fix, đặc biệt category I-J cho 5 sai sản phẩm + bịa số liệu
- 5 content templates trong `content-templates/`:
  - `facebook-caption.md` (8 templates)
  - `email-marketing.md` (6 templates)
  - `email-b2b-quote.md` (4 templates formal)
  - `product-description.md` (3 variants)
  - `landing-hero.md` (3 templates + 4 patterns)

### Verified facts (sửa từ brand guideline cũ và AI training defaults)
- ✅ In phun kỹ thuật số (KHÔNG offset)
- ✅ Không ép MOQ — từ 100 cái (KHÔNG MOQ 500)
- ✅ Lead time 2-3 ngày sản xuất (KHÔNG 14 ngày)
- ✅ Kraft nguyên sinh nhập khẩu 100% (KHÔNG tái chế)
- ✅ Quai xoắn giấy thủ công (KHÔNG ruy băng nilon)
- ✅ Primary color xanh lá `#78bc20` (KHÔNG vàng như PDF cũ)
- ✅ Không bịa số liệu khách hàng / tên brand đối tác

### Identity decisions
- Archetype: Caregiver (primary) + Creator (secondary)
- Mission: "Xưởng in dã chiến cho khách bị các xưởng lớn lãng quên"
- Vision: Bao bì xanh "nhanh – ít – rẻ" hàng đầu Việt Nam
- 4 hàng rào KHÔNG LÀM + 4 core values
- 2 tầng "bao bì xanh" (vật lý + hệ sinh thái dòng tiền)
- 3 personas: P1 chủ shop SME, P2 B2B, P3 event organizer

### Phase 3-6 — Hoãn (làm sau khi cần)
- Phase 3: Image gen prompts + 50+ ảnh reference
- Phase 4: Industry modules (6 ngành)
- Phase 5: Master AI prompt + 4 sub-prompts
- Phase 6: Social templates + stationary + illustration

---

## [v0.0.1] — 2026-04-28

### Added
- Khởi tạo repo public `minhthuc251/hoso-brand-kit`
- Scaffold cấu trúc thư mục đầy đủ
- `SKILL.md`, `README.md`, `BRAND_KIT_DECISIONS.md`, `LICENSE`
- `archive/brand-guideline-hoso-2025.pdf`
