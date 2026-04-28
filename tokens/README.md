# Design Tokens

Single source of truth cho tất cả giá trị thiết kế (màu, font, spacing, shadow, radius). AI và developer dùng những file này thay vì hard-code.

## Files

| File | Format | Dùng cho |
|---|---|---|
| `colors.json` | DTCG schema | Màu brand + neutral + semantic — đọc bởi AI, design tool, build pipeline |
| `typography.json` | DTCG schema | Font family, scale, weight, line-height, letter-spacing |
| `spacing.json` | DTCG schema | Spacing scale, border-radius, shadow |
| `tokens.css` | CSS variables | Import trực tiếp vào web project — `var(--hoso-primary)` |

## Cách dùng — theo môi trường

### 1. Web (CSS)
```css
@import url('https://raw.githubusercontent.com/minhthuc251/hoso-brand-kit/main/tokens/tokens.css');

.button-primary {
  background: var(--hoso-primary);
  color: var(--hoso-white);
  padding: var(--hoso-space-3) var(--hoso-space-5);
  border-radius: var(--hoso-radius-md);
  font-family: var(--hoso-font-body);
  font-weight: var(--hoso-weight-semibold);
}
```

### 2. Tailwind config
```js
// tailwind.config.js
import colorTokens from './hoso-brand-kit/tokens/colors.json';

export default {
  theme: {
    extend: {
      colors: {
        'hoso-primary':      colorTokens.brand.primary.$value,
        'hoso-primary-dark': colorTokens.brand['primary-dark'].$value,
        'hoso-neutral-dark': colorTokens.neutral.dark.$value,
        // ...
      },
      fontFamily: {
        heading: ['Bricolage Grotesque', 'sans-serif'],
        body:    ['Lexend Deca', 'sans-serif'],
      },
    },
  },
};
```

### 3. Figma / Sketch
Import `colors.json` qua plugin "Tokens Studio" (Figma) hoặc thủ công dán hex codes.

### 4. AI prompt (Midjourney, etc.)
```
HOSO brand colors: primary green #78bc20, dark green #519600,
kraft brown #603a17, kraft cream #f4e6d7
```

## DTCG (Design Tokens Community Group) format

Files JSON theo [chuẩn DTCG](https://design-tokens.github.io/community-group/format/):
- `$value` chứa giá trị
- `$description` chứa mô tả
- Nested object cho semantic grouping

Format này được hỗ trợ bởi: Style Dictionary, Tokens Studio, Figma Variables, hầu hết design tool hiện đại.

## Build target khác

Cần token cho iOS/Android/React Native? Mở PR đề xuất + dùng [Style Dictionary](https://amzn.github.io/style-dictionary/) để generate.
