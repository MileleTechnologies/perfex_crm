# 🚀 Perfex CRM – Milele Technologies Customized Edition

This repository contains a customized implementation of **Perfex CRM**, built and maintained by **Milele Technologies**.  
It’s a robust, PHP-based CRM system designed to streamline business operations — from managing clients and leads to automating billing, reporting, and communication.

---

## 🏢 About Milele Technologies

**Milele Technologies (TZ)** specializes in software solutions, IT infrastructure, and digital business tools tailored for enterprise and SME use.  
Our customized Perfex CRM includes enhancements for Tanzanian business environments, multi-currency invoicing, and localized automation.

---

## 🧰 Core Features

- Client, lead, and contact management  
- Project and task tracking with milestones  
- Invoice and payment processing  
- Custom dashboards and reports  
- Multi-language and currency support  
- Email and SMS notifications  
- Stripe and local payment gateway integrations  
- Role-based user access control  
- API-ready for integrations  

---

## ⚙️ System Requirements

| Component | Minimum Version | Recommended |
|------------|----------------|--------------|
| **PHP** | 7.4 | 8.1 |
| **MySQL / MariaDB** | 5.7 / 10.2 | Latest stable |
| **Composer** | Latest | Latest |
| **Web Server** | Apache / Nginx | Apache 2.4+ |
| **PHP Extensions** | cURL, mbstring, gd, zip, openssl | ✅ |

---

## 🖥️ Local Installation (XAMPP / WAMP / Laragon)

### 1️⃣ Clone the Repository
```bash
git clone git@github.com:MileleTechnologies/perfex_crm.git
cd perfex_crm
2️⃣ Install PHP Dependencies
bash
Copy code
composer install
3️⃣ Create the Database
Open http://localhost/phpmyadmin

Create a new database: perfex_crm

4️⃣ Configure Environment
Copy the example file and update it:

bash
Copy code
cp .env.example .env
Edit .env:

env
Copy code
APP_URL=http://localhost/perfex_crm
DB_HOST=localhost
DB_DATABASE=perfex_crm
DB_USERNAME=root
DB_PASSWORD=

STRIPE_KEY=pk_test_xxxxxxxxxxxxxx
STRIPE_SECRET=sk_test_xxxxxxxxxxxxxx
✅ Make sure .env is added to .gitignore.

5️⃣ Import Database (Optional)
If you have a dump file (database.sql):

Go to phpMyAdmin → Import → select the .sql file → Execute

6️⃣ Run Locally
Start your web server and visit:

arduino
Copy code
http://localhost/perfex_crm
🔐 Default Admin Credentials
Field	Value
URL	/admin
Email	admin@example.com
Password	123456

(You should change these immediately after logging in.)

⚙️ Custom Modules Included by Milele Technologies
Module Name	Description
Tanzanian Localization	Custom tax rates, currency format, and regional date support
SMS Gateway	Integration with local Tanzanian SMS providers
Advanced Reporting	Business analytics, income vs. expenses visualization
Team Attendance	Employee attendance tracking and leave management
Auto Backup Utility	Automated database and files backup system

More modules can be activated or deactivated from the admin panel → “Modules” section.

🧩 Development Notes
Framework: CodeIgniter 3.x

Language: PHP 7+

Frontend: Bootstrap 4 / jQuery

Package Manager: Composer

Version Control: Git

Deployment: Manual or CI/CD (GitHub Actions compatible)

☁️ Deployment (Live Server)
Recommended Hosting:
cPanel or VPS (Ubuntu 20.04+)

PHP 8.1 and MySQL 8.0

Steps:
Upload all project files to your web root (e.g. /public_html or /var/www/html)

Set correct file permissions:

bash
Copy code
chmod -R 755 application/
chmod -R 777 application/config
chmod -R 777 uploads/
Update .env for live database and domain:

env
Copy code
APP_URL=https://crm.mileletechnologies.co.tz
DB_HOST=localhost
DB_DATABASE=live_db_name
DB_USERNAME=live_db_user
DB_PASSWORD=strongpassword
Run:

bash
Copy code
composer install --no-dev
php artisan optimize:clear
🧑‍💻 Team Setup & Contribution Guide
Fork this repository

Clone your fork

bash
Copy code
git clone git@github.com:yourusername/perfex_crm.git
Create a feature branch

bash
Copy code
git checkout -b feature/your-feature-name
Commit and push

bash
Copy code
git add .
git commit -m "Added new feature"
git push origin feature/your-feature-name
Open a Pull Request for review

Team Standards
Follow PSR-12 PHP coding standards

Keep commit messages clear and descriptive

Never push .env or credentials

Test locally before merging to main

🧹 .gitignore Essentials
bash
Copy code
# Environment
.env
.env.*

# Dependencies
/application/vendor/
node_modules/

# OS / IDE
.DS_Store
Thumbs.db
.vscode/
.idea/
🪪 License
© 2025 Milele Technologies
This project is licensed for private and internal company use only.
Perfex CRM base license: https://www.perfexcrm.com/license

📞 Support & Contact
Milele Technologies
📧 Email: mileletechnologiestz@gmail.com
🌐 Website: https://github.com/MileleTechnologies
📍 Arusha, Tanzania

“Simplify your workflow, empower your business.”
— Milele Technologies Team
