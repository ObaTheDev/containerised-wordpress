# Containerised-wordpress

# WordPress with Docker Compose (DevOps Mini Project)

## Project Overview
This project demonstrates a **microservices-style architecture** using **Docker Compose**.  
We deploy a **WordPress site** powered by:
- **MariaDB** (database service)  
- **Volumes** for persistent storage  
- **Custom Docker networks** for inter-container communication  

This showcases **DevOps principles** such as containerization, orchestration, and reproducible environments.

---

## Architecture
```text
+---------------------+
|  WordPress (PHP)    |
|  - Exposed on :8080 |
+---------------------+
           |
           v
+---------------------+      
|   MariaDB Database  |
|  - Data persisted   |      
+---------------------+   
           |
           v
       Docker Volume (data persistence)
````

---


### 1. Clone Repository

```bash
git clone https://github.com/ObaTheDev/containerised-wordpress.git
cd containerised wordpress
```

### 2. Start Containers

```bash
docker-compose up -d
```

### 3. Access Services

* WordPress → [http://localhost:8080](http://localhost:8080)

---

## Key Concepts Demonstrated

* **Docker Compose** → service orchestration via YAML
* **Networking** → containers communicating internally by service name
* **Volumes** → persistent storage for MariaDB data and WordPress uploads
* **Port Mapping** → exposing services to host machine

---

## Screenshots

* `docs/screenshots/docker-up.png` → WordPress & MySQL containers running
* `docs/screenshots/wordpress-site.png` → WordPress setup wizard

---

## 👨‍💻 Author

**ObaTheDev**
☁️ AWS Cloud Engineer | DevOps Enthusiast

* GitHub: [@ObaTheDev](https://github.com/ObaTheDev)
* LinkedIn: [LinkedIn Profile](https://linkedin.com/in/obathedev)


