# Mongo_DB-1
this repository contains solutions to different MongoDB problems given as part of practice/assignment work

🚀 About the Project

This repository provides hands-on MongoDB exercises covering:

CRUD Operations (Create, Read, Update, Delete)
Query Filtering
Projection
Sorting
Aggregation Framework
Indexing

Each problem simulates a real-world system, making it ideal for:

📚 Students
💻 Beginners in MongoDB
🎓 Viva & Interview preparation
📚 Problem Domains

The mini projects span across multiple domains:

☕ Coffee Shop System
📞 Contact Book
✅ Task Manager
💰 Expense Tracker
🎬 Movie Watchlist
🏨 Hostel Management
🚗 Parking System
🎁 Gift Cards
📦 Courier Tracking
🏋️ Fitness Logger
📊 Subscription System
🗳️ Polling Platform
🚕 Cab Booking
🏥 Hospital System
🛒 E-commerce Wishlist
✈️ Travel Planner
📦 Inventory Management
🎵 Playlist Manager
🏦 Loan System
🍔 Delivery Tracking
⭐ Feedback System
🎟️ Ticket Booking
📱 Social Analytics
🏭 Defect Tracking

…and more.

🛠️ Tech Stack
MongoDB
Mongo Shell / Compass
(Optional) Node.js for integration
📂 How to Use
1️⃣ Clone the Repository
git clone https://github.com/ananyalytics/mongodb-mini-projects.git
cd mongodb-mini-projects
2️⃣ Start MongoDB

Make sure MongoDB is running locally or use MongoDB Atlas.

3️⃣ Open Mongo Shell
mongosh
4️⃣ Create Database
use mini_projects
5️⃣ Run Queries

Execute queries from each problem step-by-step.

🧪 Example
// Insert multiple menu items
db.menu.insertMany([
  { item_id: 1, name: "Espresso", category: "Coffee", price: 120, availability: true },
  { item_id: 2, name: "Green Tea", category: "Tea", price: 100, availability: true }
])

// Find available items
db.menu.find({ availability: true })

// Projection
db.menu.find({}, { name: 1, price: 1, _id: 0 })
🎯 Learning Outcomes

By working through this repository, you will:

Understand MongoDB fundamentals
Gain real-world database experience
Learn efficient querying techniques
Prepare for technical interviews & viva exams
📌 Who Should Use This?
Beginners learning MongoDB
Students doing DBMS labs
Developers practicing NoSQL concepts
🤝 Contributing

Contributions are welcome!

Add solutions
Optimize queries
Improve documentation
⭐ Show Your Support

If you like this repo:

⭐ Star it
🍴 Fork it
📢 Share it
📜 License


//B1 Set 2

🚀 About

This problem set is designed to strengthen your understanding of:

MongoDB CRUD operations
Query operators ($gt, $lt, $eq)
Projection
Sorting
Update operations (updateOne, updateMany)
Delete operations

These problems simulate real-world use cases, making them perfect for practice, assignments, and viva preparation.

📚 Problem List
1️⃣ Student Admission System
Manage student records in a college
Insert single & multiple records
Retrieve by department
Update contact details
Delete student data
2️⃣ Product Inventory System
Store product details
Retrieve specific fields using projection
Sort products by price
Update stock quantity
Delete expired products
3️⃣ Hospital Patient Management
Store patient records
Filter patients using age ($gt)
Display selected fields
Update discharge status
Remove archived records
4️⃣ Online Bookstore Orders
Manage customer orders
Filter by order amount ($lt)
Sort orders (descending)
Update delivery status
Delete canceled orders
5️⃣ Employee Attendance System
Track employee attendance
Filter by department ($eq)
Display specific fields
Update attendance status
Remove duplicate records
🛠️ Tech Stack
MongoDB
Mongo Shell / MongoDB Compass
▶️ How to Use
1. Start MongoDB

Make sure MongoDB is installed and running.

2. Open Mongo Shell
mongosh
3. Create Database
use set2_mongodb
4. Run Queries

Execute each problem step-by-step from the file.

🧪 Sample Code
// Insert student
db.students.insertOne({
  student_id: 101,
  name: "Rahul Sharma",
  department: "Computer Science",
  year: 2025,
  contact: "9876543210",
  city: "Bangalore"
})

// Find students from CS department
db.students.find({ department: "Computer Science" })

// Update contact
db.students.updateOne(
  { student_id: 101 },
  { $set: { contact: "9999999999" } }
)

// Delete record
db.students.deleteOne({ student_id: 105 })
🎯 Learning Outcomes

After completing this set, you will:

Understand MongoDB query operators
Perform real-world data manipulation
Improve database design thinking
Be ready for lab exams, viva & interviews
🤝 Contributing

You can:

Add solutions for each problem
Optimize queries
Improve documentation
📜 License

This content is based on GUVI materials and is intended for educational purposes only.

Free to use for educational purposes.

