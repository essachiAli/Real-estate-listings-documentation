# Laravel Deployment – Configuration Basics

## 🎯 What you will learn in this presentation

* What deployment means
* Why configuration is important
* What must be configured before deploying a Laravel project
* Common mistakes beginners make

---

## 1️⃣ What is Deployment?

Deployment is the process of moving your Laravel project from your local machine to a server so it becomes accessible online.

📌 Example:

* Local: [http://localhost](http://localhost)
* Production: [https://mywebsite.com](https://mywebsite.com)

---

## 2️⃣ Why is Configuration Important?

By default, Laravel is configured for development.
If you deploy it without proper configuration:

* Errors will be visible to users
* Security will be weak
* Performance will be poor

➡️ That is why correct configuration is required before deployment.

---

## 3️⃣ The .env File (Core Configuration)

The `.env` file contains all sensitive and environment-specific settings.

### Important settings:

```env
APP_ENV=production
APP_DEBUG=false
APP_URL=https://domain.com
```

🔴 `APP_DEBUG` must be `false` in production.

---

## 4️⃣ APP_KEY

Laravel uses `APP_KEY` to encrypt and secure data.

If it is missing:

```bash
php artisan key:generate
```

⚠️ Without an APP_KEY, the application will not work correctly.

---

## 5️⃣ Database Configuration

In the `.env` file:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_DATABASE=dbname
DB_USERNAME=dbuser
DB_PASSWORD=dbpassword
```

After that, run migrations:

```bash
php artisan migrate --force
```

---

## 6️⃣ Permissions (Very Common Issue)

Laravel needs write access to these folders:

* storage/
* bootstrap/cache/

```bash
chmod -R 775 storage bootstrap/cache
```

If permissions are incorrect, the website will not work.

---

## 7️⃣ Public Folder (Document Root)

The server document root must point to the `public` folder.

❌ Root = project/
✅ Root = project/public/

This is a very common mistake, especially on shared hosting.

---

## 8️⃣ Cache & Performance Optimization

In production, caching should be enabled:

```bash
php artisan config:cache
php artisan route:cache
php artisan view:cache
```

➡️ This significantly improves performance.

---

## 9️⃣ Storage Link (File Uploads)

If the project uses file uploads:

```bash
php artisan storage:link
```

---

## 🔥 Common Beginner Mistakes

* Forgetting to set `APP_DEBUG=false`
* Incorrect folder permissions
* Database not configured properly
* Document root not pointing to `public`
* Cache not enabled

---

## ✅ Pre‑Deployment Checklist

✔ `.env` configured
✔ `APP_ENV=production`
✔ `APP_DEBUG=false`
✔ Database connected
✔ Correct permissions
✔ Document root = `public`

---

## 🧠 Conclusion

Deployment is not just uploading files.
Proper configuration is what makes the difference between a broken website and a stable production application.

💡 Laravel is powerful, but only when correctly configured.

---

🙏 Thank you
