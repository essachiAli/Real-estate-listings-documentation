# **Slide 1: Title Slide**

**Title:** Understanding Web Deployment & Hosting
**Subtitle:** Laravel Deployment Demonstration
**Your Name / Course / Date**
Visual: Hosting + Laravel logos

---

# **Slide 2: What is Deployment?**

* Definition: Moving an application from **development environment** to **production environment**
* Purpose:

  * Make the app accessible to users
  * Ensure stability and performance
* Example: Local Laravel project → Hosted online

---

# **Slide 3: Key Deployment Concepts**

* **Production vs Development environment**
* **Web server & hosting**
* **Database connection**
* **Environment variables (.env)**
* **File permissions & security**

Visual: diagram showing local → server → users

---

# **Slide 4: Types of Hosting Services**

| Type                             | Description                           | Example             |
| -------------------------------- | ------------------------------------- | ------------------- |
| **Shared Hosting**               | Multiple websites on one server       | Hostinger, Bluehost |
| **VPS (Virtual Private Server)** | Dedicated resources, more control     | DigitalOcean, Vultr |
| **Cloud Hosting**                | Scalable resources, high availability | AWS, Google Cloud   |
| **Dedicated Hosting**            | Full server for one user              | OVH, HostGator      |

Visual: server icons / comparison chart

---

# **Slide 5: Shared Hosting vs VPS vs Cloud**

* **Shared Hosting:** Easy, cheap, limited control
* **VPS:** More control, better performance, moderate cost
* **Cloud Hosting:** Scalable, high uptime, advanced features
* **Choosing hosting depends on project needs**

Visual: simple chart comparing cost, control, scalability

---

# **Slide 6: Deployment Workflow (Conceptual)**

1. Develop locally
2. Test application
3. Upload files to hosting server
4. Configure environment (database, APP_KEY, permissions)
5. Run migrations (if needed)
6. Test online

Visual: flowchart with arrows from dev → hosting → live

---

# **Slide 7: Hosting Requirements for Laravel**

* PHP 8.1+
* MySQL / MariaDB database
* Support for `.htaccess` and mod_rewrite
* Ability to run artisan commands (optional)
* File permissions management

---

# **Slide 8: Deployment Methods**

* **Manual Upload:** File Manager / FTP (easy for shared hosting)
* **SSH / Terminal:** Composer install, artisan commands (more advanced)
* **CI/CD Pipeline:** Automated deployment (professional production)

---

# **Slide 9: Deployment Demonstration with Hostinger**

* Explain **why Hostinger** (shared hosting, easy for demonstration)
* Show **File Manager / database setup / public folder config**
* Optional: Short live demo of uploading Laravel project

---

# **Slide 10: Common Deployment Challenges**

* 500 Internal Server Error → permissions / paths
* Blank page → debug off / missing APP_KEY
* Database connection error → wrong credentials

Visual: small table with issue/solution

---

# **Slide 11: Summary & Takeaways**

* Deployment moves app from local → live server
* Hosting type impacts control, cost, and scalability
* Laravel deployment requires proper public folder, env configuration, database setup
* Hostinger demo shows practical example of deploying on shared hosting

---

# **Slide 12: References**

* Laravel Documentation: [https://laravel.com/docs](https://laravel.com/docs)
* Hostinger Knowledge Base

---

