OrderManager
This API allows users to create and manage orders.

Setup Instructions
Extract the ZIP Folder:
 - Download the project and extract the zip folder to your preferred location.

Open IntelliJ IDEA:
 - Launch IntelliJ IDEA and open the project.

Run the API:
- Run the API using IntelliJ IDEA.

Create Entities:
Use the following commands in the command prompt (CMD) to create users, items, orders, and stock movements.

1.Create User:
curl -X POST -H "Content-Type: application/json" -d "{\"name\": \"John Doe\", \"email\": \"john.doe@example.com\"}" http://localhost:8080/users

2.Create item:
curl -X POST -H "Content-Type: application/json" -d "{\"name\": \"item1\"}" http://localhost:8080/items


3.Create Order:
curl -X POST -H "Content-Type: application/json" -d "{\"creationDate\": \"2024-03-11T12:00:00\", \"itemId\": 1, \"quantity\": 0, \"userId\": 1}" http://localhost:8080/orders

4.Create Stock Movement:
curl -X POST -H "Content-Type: application/json" -d "{\"creationDate\": \"2024-03-15T12:30:00\", \"item\": {\"id\": 1}, \"quantity\": 10}" http://localhost:8080/stocks

Make sure to customize the commands as needed for your specific use case.
