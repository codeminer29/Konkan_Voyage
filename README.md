# 🌴 कोंकण VOYAGE – Travel Booking System

Welcome to **Konkan Voyage**, a full-stack web application designed for booking coastal travel packages across the Konkan region. This system allows customers to book trips, view printable tickets, and gives administrators full control to manage bookings, cancellations, and exports.

---

## 🚀 Features

### 👤 User (Passenger)

- Book destination packages via a form
- Auto-fill destination and price from package cards
- Get a **printable confirmation ticket**
- Booking status (Confirmed / Cancelled)

### 🛠 Admin

- Admin login with Spring Security
- View all bookings with table view
- Cancel or permanently delete any booking
- Export all bookings to **Excel file (.xlsx)**

---

## 🧰 Tech Stack

| Layer       | Tech Used                       |
| ----------- | ------------------------------- |
| Frontend    | HTML, CSS, Bootstrap, Thymeleaf |
| Backend     | Java, Spring Boot, Spring MVC   |
| Security    | Spring Security (Admin login)   |
| Database    | MySQL / H2 (JPA Repository)     |
| Export      | Apache POI (Excel Export)       |
| View Engine | Thymeleaf Templates             |

---

## 📁 Project Structure

```
src
├── main
│   ├── java
│   │   └── com.konkanvoyage.konkanvoyage
│   │       ├── controller
│   │       │   ├── BookingController.java
│   │       │   └── AdminController.java
│   │       ├── model
│   │       │   └── Booking.java
│   │       ├── repository
│   │       │   └── BookingRepository.java
│   │       └── config
│   │           └── SecurityConfig.java
│   └── resources
│       ├── templates
│       │   ├── index.html
│       │   ├── ticket.html
│       │   ├── login.html
│       │   └── admin-bookings.html
│       ├── static
│       │   ├── assets/
│       │   └── style.css
│       └── application.properties
```

---

## 🔐 Admin Login

> Admin login is secured using Spring Security.

- **Username**: `admin`
- **Password**: `admin123`

You can change this in `SecurityConfig.java` under the `InMemoryUserDetailsManager` bean.

---

## 🪙 How to Run Locally

1. **Clone the Repository**

```bash
git clone https://github.com/yourusername/konkan-voyage.git
cd konkan-voyage
```

2. **Start MySQL** (or use H2)

- Update your database config in `application.properties`

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/konkanvoyage
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

3. **Run the Application**

```bash
./mvnw spring-boot:run
```

4. **Visit in Browser**

- Home Page: [http://localhost:8080](http://localhost:8080)
- Admin Login: [http://localhost:8080/login](http://localhost:8080/login)

---

## 📸 Screenshots

<details>
<summary>🖼 Click to Expand</summary>

- Homepage with Packages
- Booking Form
- Admin Dashboard
- Printable Ticket View

</details>

---

## 📄 Deployment (Optional)

This app can be deployed using:

- Render (Spring Boot backend)
- Vercel / Netlify (static frontend - optional)
- PlanetScale / Railway (MySQL cloud DB)

Let me know if you want step-by-step deployment instructions.

---

## 📃 License

This project is for educational and demonstration purposes only.

---

## 🙋‍♂️ Developed By

**Soham Bamane**
🧑‍💻 Java Full-Stack Developer
📧 codeminer29@gmail.com
🌐 LinkedIn: https://www.linkedin.com/in/soham-bamane-1637602a0/
🌐 GitHub: https://github.com/codeminer29
