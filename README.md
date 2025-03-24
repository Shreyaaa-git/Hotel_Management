# Hotel Management System - README

## 🛎️ **Project Name:** Hotel Management System  
This is a Java-based **Hotel Management System** that allows users to book rooms, order food, check room availability, generate bills, and deallocate rooms. The project uses **object serialization** to save and load the hotel data for persistence.

---

## 🚀 **Features**
1. **Room Booking:**
   - Book luxury or deluxe rooms (single or double occupancy).
   - Collects customer details like name, contact number, and gender.
   - Prevents booking of already allocated rooms.

2. **Food Ordering:**
   - Allows customers to order food items with different prices.
   - Adds food charges to the final bill.

3. **Billing:**
   - Generates a detailed bill including room charges and food costs.
   - Displays the total amount payable.

4. **Room Deallocation (Checkout):**
   - Deallocates rooms upon checkout.
   - Displays the final bill before deallocation.

5. **Availability Check:**
   - Displays the number of available rooms by type.

6. **Data Persistence:**
   - Uses **serialization** to save room and customer data to a file (`backup`).
   - Restores the previous state upon reopening the application.

---

## 💻 **Technologies Used**
- **Programming Language:** Java  
- **Serialization:** `ObjectOutputStream` and `ObjectInputStream` for data persistence  
- **File I/O:** `FileInputStream`, `FileOutputStream`  
- **Multithreading:** To write data to the backup file in a separate thread  
- **Exception Handling:** Handles invalid inputs, room unavailability, and null pointer exceptions gracefully  

---

## 📁 **File Structure**
```
├── Main.java          # Main entry point of the application
├── backup             # Serialized file to store hotel data
├── README.md          # Project documentation
```

---

## ⚙️ **How to Run the Project**
1. **Compile and Run:**
   - Compile the project using the following command:
   ```
   javac Main.java
   ```
   - Run the program:
   ```
   java Main
   ```

2. **Functionality:**
   - Choose from the available options:
     - `1`: Display room details  
     - `2`: Check room availability  
     - `3`: Book a room  
     - `4`: Order food  
     - `5`: Checkout and deallocate the room  
     - `6`: Exit the program  

---

## 🍴 **Food Menu**
- `1. Sandwich` – ₹50  
- `2. Pasta` – ₹60  
- `3. Noodles` – ₹70  
- `4. Coke` – ₹30  

---

## 🛏️ **Room Types and Charges**
- **Luxury Double Room**  
  - Double bed, AC, free breakfast  
  - ₹4000 per day  
- **Deluxe Double Room**  
  - Double bed, no AC, free breakfast  
  - ₹3000 per day  
- **Luxury Single Room**  
  - Single bed, AC, free breakfast  
  - ₹2200 per day  
- **Deluxe Single Room**  
  - Single bed, no AC, free breakfast  
  - ₹1200 per day  

---

## ⚠️ **Exceptions Handled**
- **NotAvailable:** Thrown when trying to book an already occupied room.  
- **NullPointerException:** Thrown when attempting to order food in a room that is not booked.  
- **Invalid Input:** Handles invalid room numbers and menu selections gracefully.  

---

## 🛠️ **Future Enhancements**
- Add customer feedback and rating system.  
- Implement graphical user interface (GUI) for better user experience.  
- Include more food items and dynamic pricing.  
- Add payment gateway simulation for real-time transactions.  
- Integrate with a database for improved data management.

---

## 📝 **Author**
**Shreya Chakraborty**  
- Computer Science and Engineering Student  
- Software Development Enthusiast  
- Proficient in Java, Python, and Full-Stack Development  
