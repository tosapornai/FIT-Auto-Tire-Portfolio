# FIT Auto · Tire Portfolio Dashboard

Dashboard ติดตามยอดขาย ยอดซื้อ เป้า และสต็อกยางรถยนต์ FIT Auto (ข้อมูลถึง ก.ย. 2026)

## ไฟล์ในโฟลเดอร์นี้
| ไฟล์ | หน้าที่ |
|---|---|
| `index.html` | หน้า Dashboard (ฝังข้อมูลล่าสุดไว้ในไฟล์แล้ว เปิดได้ทันที) |
| `data.json` | ยอดขาย ยอดซื้อ และเป้า |
| `stock.json` | สต็อกที่สาขา |
| `loc.json` | ข้อมูลและพิกัดสาขา (ใช้คำนวณการโอนย้าย) |
| `vercel.json` | ตั้งค่า Vercel (ไม่ให้ search engine เก็บหน้า และไม่ cache ไฟล์ข้อมูล) |
| `robots.txt` | กันไม่ให้ search engine เก็บหน้า |

หน้าเว็บจะอ่าน `data.json` / `stock.json` / `loc.json` ที่วางคู่กันก่อน ถ้าไม่มีจะใช้ข้อมูลที่ฝังอยู่ใน `index.html`

## อัปเดตข้อมูลรายเดือน
1. เปิด Dashboard → กด **อัปเดตข้อมูล** → เลือกไฟล์ Excel (ยอดขาย/ยอดซื้อ/เป้า, สต็อก หรือข้อมูลสาขา)
2. กด **ดาวน์โหลดไฟล์ข้อมูล (.json)** จะได้ `data.json` หรือ `stock.json` หรือ `loc.json`
3. อัปโหลดไฟล์นั้นทับไฟล์เดิมใน GitHub (Add file → Upload files → Commit)
4. Vercel จะ deploy ใหม่อัตโนมัติภายใน 1–2 นาที

> ไม่ต้องอัปโหลดไฟล์ Excel ต้นฉบับขึ้น GitHub (`.gitignore` กันไว้แล้ว)
