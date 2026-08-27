# Template — Landing Hero Section HOSO

> Template cho hero section landing page. Khách lần đầu thấy HOSO — phải truyền tải positioning trong 5 giây.
>
> **Tất cả templates đã align với positioning đúng:** "nhanh-ít-rẻ" · in phun KTS · không ép MOQ · 2-3 ngày · xưởng dã chiến cho khách bị bỏ rơi.

## Cấu trúc chuẩn 1 hero section

```
{{Eyebrow / kicker (optional)}}
{{Headline H1 — value proposition cho persona (không phải mô tả HOSO)}}
{{Subheadline 1-2 câu — expand value + 4 facts đúng}}
{{Primary CTA}} · {{Secondary CTA}}
{{Trust indicators — số liệu thật / proof points / chứng nhận}}
```

---

## T1 — Hero cho landing chính (homepage)

### Plain text version

```
[Eyebrow] Bao bì giấy in logo "nhanh – ít – rẻ"

[H1] Xưởng in dã chiến cho shop SME, doanh nghiệp và event — từ 100 túi, sản xuất 2-3 ngày

[Subheadline]
HOSO chuyên túi giấy kraft nguyên sinh + in phun kỹ thuật số theo logo của bạn. Không ép MOQ — đơn 100 cái cũng làm. Gửi mẫu test miễn phí trước khi đặt.

[Primary CTA]   Inbox HOSO để được tư vấn
[Secondary CTA] Xem catalog

[Trust]
Top 1 Shopee bao bì giấy · Sản xuất 2-3 ngày · Mẫu test miễn phí
```

### HTML markup gợi ý

```html
<section class="hero">
  <p class="eyebrow">Bao bì giấy in logo "nhanh – ít – rẻ"</p>
  <h1>Xưởng in dã chiến cho shop SME, doanh nghiệp và event — từ 100 túi, sản xuất 2-3 ngày</h1>
  <p class="subheadline">
    HOSO chuyên túi giấy kraft nguyên sinh + in phun kỹ thuật số theo logo của bạn.
    Không ép MOQ — đơn 100 cái cũng làm. Gửi mẫu test miễn phí trước khi đặt.
  </p>
  <div class="cta-group">
    <a class="btn-primary" href="#contact">Inbox HOSO để được tư vấn</a>
    <a class="btn-secondary" href="/catalog">Xem catalog</a>
  </div>
  <div class="trust">
    <span>Top 1 Shopee bao bì giấy</span>
    <span>Sản xuất 2-3 ngày</span>
    <span>Mẫu test miễn phí</span>
  </div>
</section>
```

---

## T2 — Hero theo persona

### Cho P1 — Chủ shop SME

```
[Eyebrow] Cho shop mới mở — không cần đặt nhiều

[H1] In túi 100 cái cũng làm — sản xuất 2-3 ngày, không ép số lượng

[Subheadline]
Mới mở shop, vốn còn ít? HOSO không bắt bạn đặt 1.000 túi rồi vứt 700 cái không dùng hết. Đặt từ 100 cái, in logo theo design của bạn, sản xuất 2-3 ngày. Mẫu test miễn phí.

[Primary CTA]   Inbox HOSO — báo giá lô đầu
[Secondary CTA] Xem cách shop khác đã làm

[Trust]
100 cái cũng làm · Top 1 Shopee · Mẫu miễn phí trước khi đặt
```

### Cho P2 — Mua hàng B2B

```
[Eyebrow] Cho doanh nghiệp B2B

[H1] Bao bì in logo cho doanh nghiệp — minh bạch giấy tờ, đầy đủ VAT

[Subheadline]
HOSO làm túi giấy in logo cho doanh nghiệp B2B với hợp đồng rõ ràng, hóa đơn VAT đầy đủ, công nợ theo thỏa thuận. Sản xuất 2-3 ngày. Báo giá chính thức trong 24h sau khi nhận brief.

[Primary CTA]   Yêu cầu báo giá chính thức
[Secondary CTA] Xem chính sách công nợ

[Trust]
Đầy đủ VAT · Hợp đồng minh bạch · Sản xuất 2-3 ngày
```

### Cho P3 — Event organizer

```
[Eyebrow] Cứu hỏa event gấp

[H1] Sếp vừa quyết event tuần này — HOSO làm kịp được

[Subheadline]
HOSO chuyên cứu hỏa đơn gấp cho HR và người tổ chức event. Sản xuất 2-3 ngày, giao trực tiếp trong nội thành. File logo gửi 16h hôm nay → mai duyệt → chiều mai có hàng.

[Primary CTA]   Gọi HOSO 0348 989 949 — quyết trong 15 phút
[Secondary CTA] Xem case event đã từng làm

[Trust]
Sản xuất 2-3 ngày · Giao tận nơi · Có lưu kho miễn phí giữa các event
```

---

## T3 — Hero theo mùa / campaign

### Tết Nguyên Đán

```
[Eyebrow] Tết 2026 — chuẩn bị từ bây giờ

[H1] Túi Tết HOSO — bao bì kể chuyện cho món quà bạn trao người thân yêu

[Subheadline]
Túi Tết kraft nguyên sinh, in phun KTS hoa văn cổ truyền tùy biến theo logo của bạn. Đặt sớm để có thời gian tinh chỉnh design + duyệt mẫu test — không phải vì lo "hết slot".

[Primary CTA]   Inbox HOSO — xem mẫu túi Tết
[Secondary CTA] Đặt mẫu in test miễn phí

[Trust]
Sản xuất siêu tốc · Tinh chỉnh design miễn phí · Giao toàn quốc
```

---

## Headline patterns hiệu quả cho HOSO

### Pattern 1: "Đối tượng + Speed/MOQ promise"
> *Xưởng in dã chiến cho shop SME, doanh nghiệp và event — từ 100 túi, sản xuất 2-3 ngày*

### Pattern 2: "Pain + Counter promise"
> *Mới mở shop, vốn còn ít? HOSO không bắt bạn đặt 1.000 túi*

### Pattern 3: "Câu nói khách + HOSO trả lời"
> *Sếp vừa quyết event tuần này — HOSO làm kịp được*

### Pattern 4: "Outcome metaphor + Differentiator"
> *Bao bì in logo cho doanh nghiệp — minh bạch giấy tờ, đầy đủ VAT*

---

## Headline patterns CẤM (sai giọng HOSO)

❌ "**HOSO — Số 1 thị trường bao bì giấy Việt Nam**" (sale rởm + tuyên bố tuyệt đối)
❌ "**Giải pháp bao bì hàng đầu thế giới với công nghệ tiên tiến**" (dịch máy + overclaim)
❌ "**Mua ngay kẻo lỡ — giảm giá khủng**" (sale rởm + fake urgency)
❌ "**Bao bì giấy XỊN nhất 2026**" (tiếng lóng)
❌ "**Tại sao bạn nên chọn HOSO?**" (clickbait + tự đặt câu hỏi rỗng)
❌ "**Bao bì giấy 100% xanh, hoàn toàn không gây hại**" (overclaim eco)
❌ "**MOQ 500 — Lead time 14 ngày — In offset chuyên nghiệp**" (sai 3 facts cốt lõi!)
❌ "**Đồng hành cùng 300+ thương hiệu Việt**" (bịa số liệu)

---

## Rule cho Hero section

1. **Headline tối đa 14 từ** — đọc trong 2 giây
2. **Subheadline tối đa 35 từ** — đọc trong 5 giây
3. **CTA primary là verb-driven** — "Inbox HOSO", "Yêu cầu báo giá", "Gọi HOSO 0348 989 949"
4. **CTA secondary là explore** — "Xem catalog", "Xem case", "Tải template"
5. **Trust indicators luôn có 3** — proof points THẬT (Top 1 Shopee, 2-3 ngày, mẫu miễn phí)
6. **0 emoji trong hero** — web/landing không dùng emoji
7. **Headline có thể nhắc HOSO 1 lần** + mission "xưởng dã chiến"
8. **Bám 4 facts đúng** — kraft nguyên sinh, in KTS, không ép MOQ, 2-3 ngày
9. **KHÔNG bịa proof points** — không "300+", chỉ dùng số liệu vault confirm

---

## Checklist trước khi launch hero

- [ ] Headline ≤ 14 từ, đọc trong 2 giây
- [ ] Subheadline expand value, có proof từ vault (số liệu / chứng nhận / case)
- [ ] Primary CTA là action, có verb
- [ ] Secondary CTA cho khách "thám hiểm" thay vì commit
- [ ] 3 trust indicators bên dưới CTA — số liệu THẬT
- [ ] Không pattern cấm (xem trên)
- [ ] Mobile responsive — headline không bị xuống dòng quá nhiều
- [ ] Test reading: cho 5 người đọc trong 5 giây — ít nhất 4/5 nắm được "HOSO làm gì + cho ai"
- [ ] Có **in phun KTS** (không phải offset)
- [ ] Có **không ép MOQ** hoặc **từ 100 cái** (không phải MOQ 500)
- [ ] Có **2-3 ngày** (không phải 14 ngày)
