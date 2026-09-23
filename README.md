# Lazyweb Skills

รวม 6 skill packages ของ Lazyweb ไว้ในโฟลเดอร์ `skills/` โดยแต่ละ skill ใช้ข้อมูลจาก Lazyweb MCP (screenshot database, flows, experiments) เพื่อช่วยงานออกแบบ

## Skills

### `lazyweb-add-inspo-source`
เชื่อมต่อแหล่งแรงบันดาลใจภายนอก (Mobbin, Savee, Dribbble, Behance ฯลฯ) เข้ากับ Lazyweb design skills ทุกตัว โดย authenticate ผ่าน headless browser, เก็บ session cookie ไว้ใช้ซ้ำ และลงทะเบียนแหล่งข้อมูลนั้นให้ถูกค้นหาโดยอัตโนมัติร่วมกับ Lazyweb ในครั้งต่อไป
**ใช้เมื่อ:** ต้องการเพิ่มแหล่งอ้างอิงดีไซน์ใหม่ เช่น "add inspo source", "connect Mobbin", "link Behance"

### `lazyweb-remove-inspo-source`
ตรงข้ามกับตัวข้างบน — แสดงรายการแหล่งแรงบันดาลใจที่เชื่อมต่อไว้ และลบแหล่งที่เลือกออกจาก Lazyweb design skills
**ใช้เมื่อ:** ต้องการยกเลิกการเชื่อมต่อแหล่งข้อมูล เช่น "remove inspo source", "disconnect Mobbin"

### `lazyweb-design-brainstorm`
Skill สำหรับ brainstorm ไอเดียดีไซน์แบบ cross-pollination คือค้นหาแรงบันดาลใจจากนอกหมวดหมู่ที่ชัดเจน (domain ที่ไม่มีใครในสายงานเดียวกันมองหา) เพื่อได้แพทเทิร์นที่แปลกใหม่ไปประยุกต์ใช้
**ใช้เมื่อ:** อยากได้ไอเดียนอกกรอบ เช่น "brainstorm design ideas", "think outside the box", "surprise me"

### `lazyweb-design-improve`
รับภาพหน้าจอดีไซน์ปัจจุบันของผู้ใช้ ค้นหาหน้าจอที่คล้ายกันใน Lazyweb แล้วสร้างข้อเสนอปรับปรุงที่มีตัวอย่างอ้างอิงจริงรองรับ
**ใช้เมื่อ:** มีดีไซน์อยู่แล้วและต้องการ feedback/คำแนะนำปรับปรุง เช่น "improve this design", "design review", "compare my design to"

### `lazyweb-design-research`
วิจัยดีไซน์แบบเจาะลึก ผสมผสานข้อมูลจาก Lazyweb screenshot database กับการค้นหาบนเว็บ แล้วสรุปออกมาเป็นรายงานวิจัยที่มีโครงสร้าง พร้อมดาวน์โหลดภาพอ้างอิงมาให้
**ใช้เมื่อ:** ต้องการวิเคราะห์คู่แข่งหรือ best practice เช่น "best practices for", "competitive analysis for", "what do top apps do"

### `lazyweb-quick-references`
ค้นหาภาพหน้าจอแอปและตัวอย่าง UI แบบรวดเร็ว ดาวน์โหลดผลลัพธ์มาเก็บไว้ในเครื่องและจัดกลุ่มตามแพทเทิร์น โดยไม่ต้องทำรายงานวิจัยแบบเต็ม
**ใช้เมื่อ:** ต้องการดูตัวอย่างเร็ว ๆ เช่น "show me examples of", "UI reference for", "find screenshots of"

## โครงสร้างโฟลเดอร์

```
skills/
├── lazyweb-add-inspo-source/
├── lazyweb-design-brainstorm/
├── lazyweb-design-improve/
├── lazyweb-design-research/
├── lazyweb-quick-references/
└── lazyweb-remove-inspo-source/
```

แต่ละโฟลเดอร์มีไฟล์ `SKILL.md` ที่กำหนด metadata (`name`, `description`, `allowed-tools`) และ workflow ของ skill นั้น ๆ
