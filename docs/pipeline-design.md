# DevOps Pipeline Design

## 3.1 การพัฒนาและทดสอบอัตโนมัติ
ใช้ GitHub Actions ในการ run test อัตโนมัติทุกครั้งที่มี push

## 3.2 Containerize และ Deploy
ใช้ Docker สร้าง container และ Kubernetes ในการ deploy
- ใช้ LoadBalancer service
- ตั้งค่า Horizontal Pod Autoscaler

## 3.3 การตรวจสอบผลการทดสอบ
- Defect Criteria: หาก test ไม่ผ่านให้หยุด deploy
- Exit Criteria: test ต้องผ่านทั้งหมดก่อน merge

## 3.4 ตรวจสอบคู่มือการใช้งาน
- มีเอกสารการใช้งานระบบเบื้องต้น
