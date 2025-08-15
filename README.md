# DCP Fonts CDN (ฟรีด้วย GitHub + jsDelivr)

โครงสร้างนี้พร้อมใช้งาน: อัปโหลดขึ้น GitHub แล้วเรียก `fonts.css` ผ่าน jsDelivr ได้เหมือน Google Fonts

## โครงสร้าง
```
/
├─ fonts/                                  # (มีไฟล์ .woff2/.woff ที่แปลงแล้ว)
├─ fonts.css
└─ example.html
```

## ขั้นตอน
1) อัปโหลดทั้งหมดขึ้น GitHub Repo ของคุณ
2) เรียกผ่าน jsDelivr:
```
https://cdn.jsdelivr.net/gh/USERNAME/REPO/fonts.css
```
> เปลี่ยน USERNAME/REPO ให้ตรงของคุณ

## ใช้งาน
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/USERNAME/REPO/fonts.css">
```
```css
body { font-family: 'DCPText', sans-serif; }
```

## หมายเหตุ
- ตั้ง `font-display: swap;` แล้ว เพื่อประสบการณ์โหลดที่ดี
- ถ้าต้องการระบุ subset ให้เติม `unicode-range` ในแต่ละ @font-face
- หากเพิ่มน้ำหนัก/สไตล์ใหม่ ให้คัดลอกบล็อก @font-face แล้วแก้ไฟล์/น้ำหนักตามจริง
