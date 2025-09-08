<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c4be907703b836d1a1c360db20da4de9",
  "translation_date": "2025-08-29T16:15:00+00:00",
  "source_file": "11-agentic-protocols/code_samples/github-mcp/MCP_SETUP.md",
  "language_code": "th"
}
-->
# คู่มือการเชื่อมต่อ MCP Server

## ข้อกำหนดเบื้องต้น
- ติดตั้ง Node.js (เวอร์ชัน 14 ขึ้นไป)
- ตัวจัดการแพ็กเกจ npm
- สภาพแวดล้อม Python พร้อม dependencies ที่จำเป็น

## ขั้นตอนการตั้งค่า

1. **ติดตั้ง MCP Server Package**  
   ```bash
   npm install -g @modelcontextprotocol/server-github
   ```

2. **เริ่มต้น MCP Server**  
   ```bash
   npx @modelcontextprotocol/server-github
   ```  
   เซิร์ฟเวอร์ควรเริ่มทำงานและแสดง URL การเชื่อมต่อ

3. **ตรวจสอบการเชื่อมต่อ**  
   - มองหาไอคอนปลั๊ก (🔌) ในอินเทอร์เฟซ Chainlit  
   - ควรมีตัวเลข (1) ปรากฏข้างไอคอนปลั๊กเพื่อแสดงว่าการเชื่อมต่อสำเร็จ  
   - คอนโซลควรแสดงข้อความ: "GitHub plugin setup completed successfully" (พร้อมกับสถานะเพิ่มเติม)

## การแก้ไขปัญหา

### ปัญหาที่พบบ่อย

1. **ปัญหาพอร์ตซ้ำซ้อน**  
   ```bash
   Error: listen EADDRINUSE: address already in use
   ```  
   วิธีแก้ไข: เปลี่ยนพอร์ตโดยใช้:  
   ```bash
   npx @modelcontextprotocol/server-github --port 3001
   ```

2. **ปัญหาการยืนยันตัวตน**  
   - ตรวจสอบให้แน่ใจว่ากำหนดค่า GitHub credentials อย่างถูกต้อง  
   - ตรวจสอบว่าไฟล์ .env มีโทเค็นที่จำเป็น  
   - ยืนยันการเข้าถึง API ของ GitHub  

3. **การเชื่อมต่อล้มเหลว**  
   - ยืนยันว่าเซิร์ฟเวอร์กำลังทำงานบนพอร์ตที่คาดไว้  
   - ตรวจสอบการตั้งค่าไฟร์วอลล์  
   - ตรวจสอบว่าสภาพแวดล้อม Python มีแพ็กเกจที่จำเป็นครบถ้วน  

## การตรวจสอบการเชื่อมต่อ

เซิร์ฟเวอร์ MCP ของคุณเชื่อมต่ออย่างถูกต้องเมื่อ:  
1. คอนโซลแสดงข้อความ "GitHub plugin setup completed successfully"  
2. บันทึกการเชื่อมต่อแสดงข้อความ "✓ MCP Connection Status: Active"  
3. คำสั่ง GitHub ทำงานในอินเทอร์เฟซแชทได้

## ตัวแปรสภาพแวดล้อม

สิ่งที่ต้องมีในไฟล์ .env ของคุณ:  
```
GITHUB_TOKEN=your_github_token
MCP_SERVER_PORT=3000  # Optional, default is 3000
```

## การทดสอบการเชื่อมต่อ

ส่งข้อความทดสอบนี้ในแชท:  
```
Show me the repositories for username: [GitHub Username]
```  
การตอบกลับที่สำเร็จจะแสดงข้อมูลของ repository

---

**ข้อจำกัดความรับผิดชอบ**:  
เอกสารนี้ได้รับการแปลโดยใช้บริการแปลภาษา AI [Co-op Translator](https://github.com/Azure/co-op-translator) แม้ว่าเราจะพยายามให้การแปลมีความถูกต้องมากที่สุด แต่โปรดทราบว่าการแปลโดยอัตโนมัติอาจมีข้อผิดพลาดหรือความไม่ถูกต้อง เอกสารต้นฉบับในภาษาดั้งเดิมควรถือเป็นแหล่งข้อมูลที่เชื่อถือได้ สำหรับข้อมูลที่สำคัญ ขอแนะนำให้ใช้บริการแปลภาษามืออาชีพ เราไม่รับผิดชอบต่อความเข้าใจผิดหรือการตีความที่ผิดพลาดซึ่งเกิดจากการใช้การแปลนี้