

The Hotel Management System is a Java-based desktop application designed to automate daily hotel operations. It includes features such as customer management, room booking, billing, food ordering, check-in/check-out, and more.

This project is built using Core Java, JDBC, MySQL, and Swing/Console UI.

🎯 Features
✅ Room Management

View available rooms

Add / update rooms

Book and checkout rooms

Change room status (Booked / Free)

✅ Customer Management

Add customer details

Store complete records

Assign room numbers

View customer list

✅ Billing System

Auto billing at checkout

Includes room + food + service charges

Accurate calculation

✅ Food / Service Management

Add food orders

Track service usage

Auto add cost in bill

🛠️ Technologies Used
Layer	Technology
Language	Java
UI	Console / Swing
Database	MySQL
Connectivity	JDBC
Version Control	Git / GitHub
🗂️ Project Structure
Hotel-Management-Project
 ┣ 📂 src
 ┃ ┣ Customer.java
 ┃ ┣ Room.java
 ┃ ┣ Bill.java
 ┃ ┣ Food.java
 ┃ ┣ DatabaseManager.java
 ┃ ┗ Main.java
 ┣ 📂 database
 ┃ ┗ hotel_db.sql
 ┣ README.md
 ┗ pom.xml (optional)

⚙️ Installation & Setup
✔️ Step 1: Clone Repository
git clone https://github.com/your-username/hotel-management.git

✔️ Step 2: Install MySQL

Download from:
https://dev.mysql.com/downloads/

✔️ Step 3: Create Database
CREATE DATABASE hotel;

✔️ Step 4: Create Tables
USE hotel;

CREATE TABLE room (
  room_no INT PRIMARY KEY,
  type VARCHAR(50),
  price DOUBLE,
  status VARCHAR(20)
);

CREATE TABLE customer (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  mobile VARCHAR(20),
  room_no INT,
  checkin DATE,
  checkout DATE
);

✔️ Step 5: Configure DB Connection

Edit connection in DatabaseManager.java:

Connection con = DriverManager.getConnection(
  "jdbc:mysql://localhost:3306/hotel",
  "root",
  "password"
);

✔️ Step 6: Run Application

Open the project → run Main.java

🧪 Usage Flow

1️⃣ Customer check-in
2️⃣ Assign / book room
3️⃣ Add food or services
4️⃣ Auto bill generation
5️⃣ Checkout
6️⃣ All data stored in database

📈 Future Enhancements

✔️ Online reservation
✔️ PDF bill printing
✔️ GST / tax calculation
✔️ Admin login system
✔️ Staff salary module
✔️ Room analytics dashboard

🤝 Contributing

Pull requests are welcome!
You can also suggest improvements to enhance the project.




