# HC-SR04-ultrasonic-sensor-micropython
ไฟล์ที่จำเป็น
hcsr04.py
main.py
ssd1306.py (กรณีแสดงค่าผ่านจอ OLED)

อธิบายการทำงานของ code
1.เรียกคลาส Hcsro4 มาใช้งานจาก Hcscr04 library
2.เรียกใช้ time library มาหน่วงเวลา
3.สร้าง object ของ Hcsr04 ชื่อ sensor โดยให้มีการส่งค่าพารามิเตอร์ที่ขา Trigger/echo/กำหนดเวลาการส่งคลื่นซาวด์เวบไว้สูงสุดคือ 10000
4.นำ object ที่สร้างชื่อ sensor มากำหนดระยทางเป็นหน่วย ซม และอ่านค่า ด้วยฟังก์ชั่น distance_cm()ใน Hcsro4 library
5.แสดงค่าระยะทางเป็น ซม 
6.หน่วงเพื่อแสดงค่า 1 วินาที
