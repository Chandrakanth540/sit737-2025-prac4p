### **README.md**  

```md
# Calculator Microservice  

A simple arithmetic microservice built using **Express.js** that performs basic mathematical operations (addition, subtraction, multiplication, and division). It also includes **error handling** and **logging** using Winston.  

---

## **Features**  
✅ RESTful API with four endpoints  
✅ Handles invalid inputs and division by zero  
✅ Logs errors and operations using Winston  
✅ Lightweight and easy to extend  

---

## **Prerequisites**  
Make sure you have the following installed:  
- [Node.js](https://nodejs.org/) (v14 or later)  
- npm (comes with Node.js)  

---

## **Installation**  

1️⃣ **Clone the repository**

```sh
git [https://github.com/Chandrakanth540/sit737-2025-prac4p.git]
cd sit737-2025-prac4p
```

2️⃣ **Install dependencies**  
```sh
npm install
```

---

## **Usage**  

### **Start the Server**  
```sh
node index.js
```
Server runs on `http://localhost:3000`.

### **API Endpoints**  

| Operation  | Endpoint  | Example Request  |
|------------|------------|----------------|
| Addition | `/add` | `http://localhost:3000/add?num1=5&num2=3` |
| Subtraction | `/subtract` | `http://localhost:3000/subtract?num1=10&num2=4` |
| Multiplication | `/multiply` | `http://localhost:3000/multiply?num1=5&num2=3` |
| Division | `/divide` | `http://localhost:3000/divide?num1=6&num2=3` |

### **Example Responses**  
📌 **Addition Request:**  
```sh
curl "http://localhost:3000/add?num1=5&num2=3"
```
📌 **Response:**  
```json
{ "result": 8 }
```

📌 **Division by Zero Error:**  
```sh
curl "http://localhost:3000/divide?num1=10&num2=0"
```
📌 **Response:**  
```json
{ "error": "Cannot divide by zero." }
```

---

## **Logging**  
✅ Logs successful operations in `logs/combined.log`  
✅ Logs errors in `logs/error.log`  

---

## **Project Structure**  

```
calculator-microservice/
│── logs/                 # Stores log files  
│── index.js              # Main Express server  
│── package.json          # Dependencies and scripts  
│── README.md             # Documentation  
```

---

## **Future Enhancements**  
🔹 Deploy using Docker  
🔹 Add authentication with JWT  
🔹 Implement unit tests with Jest  

---

## **License**  
MIT License © 2025 Chandrakanth  
