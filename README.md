# Pattra Villa 8 — Parking Map

Single-file web app สำหรับจัดการที่จอดรถภายในหมู่บ้าน

- **Live URL:** https://pattra8.github.io/parking/
- **Stack:** HTML / CSS / Vanilla JS — ไม่ใช้ build tool, deploy เป็น static ได้เลย

## Files

| ไฟล์ | คำอธิบาย |
|---|---|
| `index.html` | App ทั้งหมด (UI + state + admin + visitor flow) |
| `bg.jpg` | ภาพ aerial bird's eye ของหมู่บ้าน (พื้นหลังแผนที่) |

## Features

- 🗺️ Live map พร้อมภาพ aerial จริง · 17 default slots
- 👑 Admin login — PIN `1234`
  - ➕ เพิ่ม / ✕ ลบ slot
  - ✏️ ลาก slot พร้อม **snap-to-grid 4px + smart alignment guides**
  - 📐 Auto Align — จัดทุก slot เข้าแนว row/column ทีเดียว
  - 💾 Save / ↺ Reset
- 🚗 Visitor booking + PromptPay (SCB 093-2-43819-1)
- 💾 Persist ผ่าน localStorage (รอ Firebase รอบหน้า)

## Deploy to GitHub Pages

หลัง push ไป GitHub:

1. ไปที่ repo → **Settings** → **Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main` / `/ (root)` → **Save**
4. รอ 30–60 วินาที เปิด https://pattra8.github.io/parking/

## Where this page is published (since 19 Sep 2026)

`/parking/` is served from the `parking/` folder of the
[`pattra8.github.io`](https://github.com/pattra8/pattra8.github.io) repo,
together with every other Pattra page. GitHub Pages on **this** repo is
turned off — while it was on, a project page at `pattra8.com/parking/`
shadowed that folder, so edits published to `pattra8.github.io` never went
live here. Edit `parking/index.html` in `pattra8.github.io`; this repo is
kept as the source history only.
