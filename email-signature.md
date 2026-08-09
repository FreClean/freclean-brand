# Email Signature Template

Plain-text version (universally compatible):

```
[Full Name]
[Title] · FreClean
freclean7@gmail.com · +1 (849) 388-1969
Léogâne, Ouest, Haiti
```

HTML version (uses brand colors from `../docs/02-color-system.md`):

```html
<table style="font-family: Inter, Arial, sans-serif; font-size: 13px; color: #0F2A2E;">
  <tr>
    <td style="padding-right: 12px;">
      <div style="width:40px;height:40px;border-radius:10px;background:linear-gradient(100deg,#0B72B9,#2FAE60);"></div>
    </td>
    <td>
      <strong style="font-family: 'Space Grotesk', sans-serif; font-size: 14px;">[Full Name]</strong><br>
      <span style="color:#5B7A77;">[Title] · FreClean</span><br>
      <a href="mailto:freclean7@gmail.com" style="color:#084F80;">freclean7@gmail.com</a> ·
      <a href="tel:+18493881969" style="color:#084F80;">+1 (849) 388-1969</a><br>
      <span style="color:#5B7A77;">Léogâne, Ouest, Haiti</span>
    </td>
  </tr>
</table>
```

Replace the gradient `<div>` placeholder with the real logo mark once a small-format PNG/SVG exists (see `../docs/01-logo-usage.md`).
