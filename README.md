# manage products service

This is a Java-based backend service that handles core product management operations such as creating,searching, updating, deleting, and approving or rejecting products within an application.

---

## 🚀 Features

- Create new products
- Serach products
- retrieve products
- Update existing product details
- Soft delete products
- Approve or reject product records


---

## ⚙️ Tech Stack

- Java 8+
- Spring Boot
- PostgreSQL (pluggable)
- JPA / Hibernate
- REST APIs
- Junit Framwork
- Swagger2 (for API docs)
  
---

## 📂 Project Structure

src/
├── main/
│ ├── java/
│ │ └── com/product/products/
│ │ ├── controller/
│ │ ├── entity/
│ │ ├── repository/
│ │ └── service/
│ └── resources/
│── test/java/com/product/productscreen/
   └── controller/

---

## 🛠️ Setup & Run

### 1. Clone the repository
```bash
git clone https://github.com/raja-dev-stack/manage-products-service.git
cd manage-products-service
2. Build and run
bash
Copy
Edit
./mvnw spring-boot:run
or

bash
Copy
Edit
./gradlew bootRun
3. Access the API
bash
Copy
Edit
http://localhost:8080/api/products
📑 API Endpoints
Method	Endpoint	Description
POST	product in request body 	Create a new product
GET  /api/products/search  
PUT	/api/products/{productId}	Update product by ID
DELETE	/api/products/{productId}	Delete product by ID
POST	/api/products/approval-queue/{approvalId}/approve 	Approve a product
POST /api/products/approval-queue/{approvalId}/reject    Reject a product
GET /api/products/approval-queue  Get Products in Approval Queue
GET	/api/products	List all products

🧪 Testing
Use Postman or Swagger2 UI to test the endpoints

Unit and integration tests  are located under src/test/java

📌 Notes
This service is intended to be used as a backend component of a larger application.

Approval logic can be customized based on business rules.


📝 License







