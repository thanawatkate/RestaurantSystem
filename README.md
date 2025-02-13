# Restaurant Management System

## 📌 Overview
**Restaurant Management System** เป็นโปรแกรมจัดการร้านอาหารที่ช่วยให้พนักงานสามารถดูเมนู สั่งอาหาร และจัดการคำสั่งซื้อได้อย่างมีประสิทธิภาพ โดยพัฒนาโดยใช้ **Java** และ **PostgreSQL** เป็นฐานข้อมูลหลัก

## 🛠️ Features
- 🔹 **ระบบเมนูอาหาร**: แสดงรายการอาหารจากฐานข้อมูล
- 🔹 **ระบบสั่งอาหาร**: บันทึกคำสั่งซื้อของลูกค้า
- 🔹 **ระบบจัดการพนักงาน**: เพิ่ม, ลบ, แก้ไขข้อมูลพนักงาน
- 🔹 **ระบบจัดการลูกค้า**: บันทึกข้อมูลลูกค้าและประวัติการสั่งซื้อ
- 🔹 **รองรับ GUI**: ใช้ Java Swing / JavaFX (สามารถขยายเป็น Web App ได้)

## 🏗️ Technologies Used
- **Java (JDK 8+)** - สำหรับการพัฒนา Backend และ GUI
- **PostgreSQL** - ฐานข้อมูลสำหรับจัดเก็บข้อมูล
- **JDBC** - ใช้ในการเชื่อมต่อฐานข้อมูล PostgreSQL
- **Maven (Optional)** - สำหรับจัดการ Dependencies

## 📂 Project Structure
```
/RestaurantSystem
│── src/
│   ├── database/
│   │   ├── DatabaseConnection.java      // เชื่อมต่อฐานข้อมูล
│   │
│   ├── models/  
│   │   ├── MenuItem.java               // โครงสร้างข้อมูลเมนู
│   │   ├── Order.java                  // โครงสร้างคำสั่งซื้อ
│   │
│   ├── services/
│   │   ├── MenuService.java            // จัดการข้อมูลเมนู
│   │   ├── OrderService.java           // จัดการคำสั่งซื้อ
│   │
│   ├── ui/
│   │   ├── OrderScreen.java            // GUI สำหรับสั่งอาหาร
│   │
│   ├── Main.java                        // จุดเริ่มต้นของโปรแกรม
│
│── pom.xml                              // (ถ้าใช้ Maven)
│── README.md                            // รายละเอียดของระบบ
```

## 📖 Installation & Setup
### 1️⃣ ติดตั้ง PostgreSQL และสร้างฐานข้อมูล
```sql
CREATE DATABASE restaurant_db;
```
### 2️⃣ ตั้งค่า Database Connection ใน `DatabaseConnection.java`
```java
private static final String URL = "jdbc:postgresql://localhost:5432/restaurant_db";
private static final String USER = "your_username";
private static final String PASSWORD = "your_password";
```
### 3️⃣ คอมไพล์และรันโปรแกรม
```sh
javac -d bin src/**/*.java
java -cp bin Main
```

## 🚀 Usage
1. เปิดโปรแกรมแล้วเลือกเมนูอาหาร
2. เลือกจำนวนอาหารและกด "Place Order"
3. ระบบจะบันทึกข้อมูลลงฐานข้อมูล

## 👨‍💻 Future Enhancements
- เพิ่มระบบล็อกอินพนักงาน
- รองรับ API สำหรับเชื่อมกับ Web App
- เพิ่มระบบคิดเงินอัตโนมัติ

## 📝 License
MIT License

---
✨ **Developed by [Your Name]** ✨

