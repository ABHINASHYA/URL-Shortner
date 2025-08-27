
# 🔗 URL Shortener

A simple and efficient **URL Shortener** application that converts long URLs into short, shareable links. This project demonstrates the fundamentals of backend development, database integration, and clean code practices.

---

## 🚀 Features

* Shortens long URLs into unique, compact links
* Redirects users from the short link to the original URL
* Stores and retrieves URL mappings using a database
* Input validation for URLs
* Easy to extend with analytics (click counts, expiration dates, etc.)

---

## 🛠️ Tech Stack

* **Language:** Java
* **Framework:** Spring Boot (if you used it, confirm) / Plain Java
* **Database:** MySQL / PostgreSQL / MongoDB (please confirm what you used)
* **Tools:** Maven / Gradle

---

## ⚙️ Installation & Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/ABHINASHYA/URL-Shortner.git
   cd URL-Shortner
   ```

2. **Build the project**

   ```bash
   mvn clean install
   ```

3. **Run the application**

   ```bash
   mvn spring-boot:run
   ```

   or

   ```bash
   java -jar target/url-shortener-0.0.1-SNAPSHOT.jar
   ```

4. **Access the app**

   * API will be available at: `http://localhost:8080`

---

## 📌 Usage

* **Shorten URL**

  ```http
  POST /shorten
  Content-Type: application/json  

  {
    "url": "https://example.com/very/long/url"
  }
  ```

  ✅ Response:

  ```json
  {
    "shortUrl": "http://localhost:8080/abc123"
  }
  ```

* **Redirect**
  Visit:

  ```
  http://localhost:8080/abc123
  ```

  ➡ Redirects to the original long URL

---

## 📂 Project Structure

```
URL-Shortner/
│── src/
│   ├── main/
│   │   ├── java/com/example/urlshortener/
│   │   │   ├── controller/
│   │   │   ├── service/
│   │   │   ├── repository/
│   │   │   └── model/
│   │   └── resources/
│   │       └── application.properties
│── pom.xml
│── README.md
```

---

## 🏗️ Future Improvements

* Add analytics (number of clicks per short URL)
* Custom short links (user-defined)
* Expiration time for short links
* Frontend UI for user interaction

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to improve.

---

## 📜 License

This project is licensed under the MIT License.
