# Day 5 - Student Management API (2025/04/08) 📚👨‍💻

## 📝 Description
This is a simple Spring Boot REST API built for managing student information. It supports basic CRUD operations, allows retrieving student details by ID, and includes additional functionality like filtering students by age and sorting them by GPA.

---

## 🗂️ Project Structure

```

src/
└── main/
└── java/
└── lk/ac/vau/fas/ict/
├── model/
│   └── Student.java           # Defines the Student entity
└── controller/
├── StudentController.java # Main controller for student operations
└── SendDataController.java # Basic data endpoint (e.g., age)

````

---

## 🧩 Models

### ✅ `Student.java`
Defines the structure of a student with the following attributes:
- `name` (String)
- `age` (int)
- `course` (String)
- `regNo` (String)
- `gpa` (double)

---

### 🔗 API Endpoints

#### 🧑‍🎓 Student Management (`/app`)

| Method | Endpoint               | Description                             |
| ------ | ---------------------- | --------------------------------------- |
| GET    | `/app/mapstudent/{id}` | Get a student by registration number    |
| GET    | `/app/mapstudentAll`   | Get all students                        |
| POST   | `/app/add`             | Add a new student                       |
| DELETE | `/app/delStu/{reg}`    | Delete a student by registration number |
| PUT    | `/app/update/{reg}`    | Update a student by registration number |

---

## 🧪 Example Usage & Outputs

### 📥 Get All Students


![2 Get All Students](https://github.com/user-attachments/assets/54ef7c53-995b-4079-9ea3-631464e7637e)

---

### 🔍 Get Student by Registration Number


![1 Get a Student by Registration Number](https://github.com/user-attachments/assets/db160649-48b5-4562-8d9b-de8f770109a2)

---

### ➕ Add New Student


![3 Add a New Student](https://github.com/user-attachments/assets/f4921dd8-3d1b-44df-9de7-1597026fc69a)

---

### ✏️ Update Student


![4 Update an Existing Student](https://github.com/user-attachments/assets/5200ee99-473f-43ba-ab8c-02def40c0de2)

---

### ❌ Delete Student


![5 Delete a Student](https://github.com/user-attachments/assets/9d6e393f-452a-4fba-9ce3-9ae78637f07f)

---

## 💾 Data Storage

The application uses in-memory `HashMap` to store student data:

* Key: Registration Number (`regNo`)
* Value: Student object

⚠️ Data will be **lost upon application restart**.

---

## 💻 Technologies Used

* **Spring Boot** 🚀
* **Spring Web** 🌐
* **Java** ☕
