# ค้นคำพิพากษาฎีกา PWA

PWA สำหรับสืบค้นคำพิพากษาศาลฎีกา เชื่อมต่อ deka.supremecourt.or.th

## ฟีเจอร์
- 🔍 ค้นด้วยคำหรือเลขที่ฎีกา
- 📌 บันทึกคำค้นที่ใช้บ่อย
- 🕐 ประวัติการค้นหา
- ⚡ ค้นด่วนด้วย preset chips
- 📱 ติดตั้งเป็น app บนมือถือได้
- 🌙 Dark mode

## วิธี deploy บน GitHub Pages

1. สร้าง repository ใหม่ใน GitHub
2. Upload ไฟล์ทั้งหมดในโฟลเดอร์นี้
3. ไปที่ Settings → Pages → Source: Deploy from branch → main → / (root)
4. เข้าใช้งานที่ `https://<username>.github.io/<repo-name>/`

## ไฟล์
```
index.html      — แอปหลัก (ไฟล์เดียว)
manifest.json   — PWA manifest
sw.js           — Service Worker (offline support)
icons/          — ไอคอน 192px และ 512px
```

## หมายเหตุ
เว็บ deka.supremecourt.or.th ใช้ระบบค้นหาแบบ POST form
PWA นี้จะเปิดเว็บในแท็บใหม่พร้อมคำค้น แต่อาจต้องกรอกคำค้นซ้ำในเว็บต้นทาง
ประวัติและคำบันทึกเก็บใน localStorage ของ browser
