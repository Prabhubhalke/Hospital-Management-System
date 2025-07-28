# 🏥 Hospital Management System

A comprehensive PHP-based Hospital Management System with patient records, appointment booking, doctor management, and administrative features.

## 📋 Table of Contents

- [Features](#-features)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Database Setup](#-database-setup)
- [Login Credentials](#-login-credentials)
- [System Structure](#-system-structure)
- [Usage](#-usage)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

### 🎯 Core Features
- **Patient Management** - Complete patient records and history
- **Doctor Management** - Doctor profiles and specializations
- **Appointment Booking** - Schedule and manage appointments
- **HIV Patient Records** - Specialized HIV patient tracking
- **Outbreak Management** - Disease outbreak monitoring
- **User Management** - Multi-level user access control
- **Dashboard Analytics** - Real-time statistics and reports

### 🔐 User Roles
- **Administrator** - Full system access
- **Doctor/Staff** - Patient and appointment management
- **Patient** - Personal records and appointment booking

## 🛠️ Requirements

### Server Requirements
- **Web Server:** Apache/Nginx
- **PHP Version:** 7.2 or higher
- **Database:** MySQL 5.6 or higher
- **Web Server:** XAMPP/WAMP/LAMP

### PHP Extensions
- PDO MySQL
- Session Support
- Cookie Support

## 📦 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/hospital-management-system.git
cd hospital-management-system
```

### 2. Web Server Setup
1. Copy the project to your web server directory:
   - **XAMPP:** `C:\xamp\htdocs\`
   - **WAMP:** `C:\wamp\www\`
   - **LAMP:** `/var/www/html/`

2. Start your web server (Apache) and MySQL services

### 3. Database Setup
1. Open phpMyAdmin: `http://localhost/phpMyAdmin`
2. Create a new database named `hospital`
3. Import the database schema from `database/hospital.sql`

### 4. Configuration
The system is pre-configured for localhost. If you need to change database settings, edit `classes/Config.class.php`:

```php
const DB_HOST = "localhost";
const DB_NAME = "hospital";
const DB_USER = "root";
const DB_PASSWORD = "";
```

## 🗄️ Database Setup

### Automatic Setup (Recommended)
```bash
# Using MySQL command line
mysql -u root -p
CREATE DATABASE hospital;
USE hospital;
SOURCE database/hospital.sql;
```

### Manual Setup
1. Create database `hospital`
2. Import `database/hospital.sql`
3. Verify all tables are created:
   - `users`
   - `patients`
   - `appointment`
   - `outbreaks`
   - `hiv`

## 🔐 Login Credentials

### Administrator Access
| Email | Password | Role |
|-------|----------|------|
| `admin@admin.com` | `admin` | Super Admin |
| `admin@hospital.com` | `admin123` | Administrator |
| `bensontesting@gmail.com` | `programming` | Admin |

### Doctor/Staff Access
| Email | Password | Role |
|-------|----------|------|
| `totonajoyce@gmail.com` | `12345` | Surgeon |
| `bensonwainaina30gmail.com` | `hospital` | Clinical Officer |

## 🏗️ System Structure

```
Hospital_Management_System/
├── classes/                 # PHP Classes
│   ├── Config.class.php    # Database configuration
│   ├── Db.class.php        # Database operations
│   ├── User.class.php      # User authentication
│   ├── Patient.class.php   # Patient management
│   └── ...
├── css/                    # Stylesheets
├── js/                     # JavaScript files
├── images/                 # System images
├── inc/                    # Include files
├── database/               # Database schema
│   └── hospital.sql
├── index.php              # Main dashboard
├── login.php              # Login page
├── importance.php         # Core initialization
└── README.md              # This file
```

## 🚀 Usage

### 1. Access the System
- **URL:** `http://localhost/Hospital_Management_System/`
- **Login Page:** `http://localhost/Hospital_Management_System/login.php`

### 2. Login Process
1. Choose your role (Admin/Doctor/Patient)
2. Enter credentials
3. Access the dashboard

### 3. Main Features
- **Dashboard:** View system statistics
- **Patients:** Manage patient records
- **Doctors:** Manage doctor profiles
- **Appointments:** Book and manage appointments
- **Reports:** Generate system reports

## 🔧 Troubleshooting

### Common Issues

#### 1. Login Not Working
- **Issue:** Login page keeps refreshing
- **Solution:** Check database connection and user credentials
- **Fix:** Verify database exists and tables are created

#### 2. Database Connection Error
- **Issue:** "Column not found" errors
- **Solution:** Import the complete database schema
- **Fix:** Run `database/hospital.sql` in phpMyAdmin

#### 3. PHP Compatibility Issues
- **Issue:** `__autoload()` deprecated error
- **Solution:** System already updated to use `spl_autoload_register()`
- **Fix:** Use PHP 7.2+ for best compatibility

#### 4. Cookie Issues
- **Issue:** Login not persisting
- **Solution:** Check browser cookie settings
- **Fix:** Enable cookies in browser settings

### Debug Tools
- **Debug Login:** `http://localhost/Hospital_Management_System/debug_login.php`
- **Direct Login:** `http://localhost/Hospital_Management_System/direct_login.php`

## 🛡️ Security Features

- **Session Management:** Secure session handling
- **Cookie Security:** HTTP-only cookies
- **SQL Injection Protection:** Prepared statements
- **Access Control:** Role-based permissions
- **Password Protection:** Secure authentication

## 📊 System Requirements

### Minimum Requirements
- **RAM:** 2GB
- **Storage:** 100MB
- **PHP Memory:** 128MB
- **Upload Limit:** 10MB

### Recommended Requirements
- **RAM:** 4GB+
- **Storage:** 500MB+
- **PHP Memory:** 256MB+
- **Upload Limit:** 50MB+

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow PHP PSR-4 autoloading standards
- Use prepared statements for database queries
- Maintain consistent code formatting
- Add comments for complex logic

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

### Getting Help
- **Documentation:** Check this README first
- **Issues:** Create an issue on GitHub
- **Email:** support@hospitalmanagement.com

### System Information
- **Version:** 1.0.0
- **Last Updated:** July 2025
- **PHP Version:** 7.2+
- **Database:** MySQL 5.6+

## 👨‍💻 Connect with Me

**Developer:** Prabhu Bhalke

- 📧 **Email:** [prabhubhalke379@gmail.com](mailto:prabhubhalke379@gmail.com)
- 🔗 **LinkedIn:** [linkedin.com/in/prabhu-bhalke-1a258625a](https://linkedin.com/in/prabhu-bhalke-1a258625a)
- 📱 **Phone:** [+91 63632 81278](tel:+916363281278)

### 🤝 Let's Connect
Feel free to reach out for:
- **Technical Support** - Help with installation or customization
- **Feature Requests** - Suggestions for new features
- **Collaboration** - Working together on projects
- **Questions** - Any queries about the system

## 🎉 Acknowledgments

- Built with PHP and MySQL
- Uses Bootstrap for responsive design
- jQuery for enhanced user experience
- PDO for secure database operations

---

**Note:** This is a development system. For production use, ensure proper security measures, SSL certificates, and regular backups are implemented. 