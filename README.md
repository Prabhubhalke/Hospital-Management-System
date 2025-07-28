# 🏥 Hospital Management System – PHP & MySQL

A role-based Hospital Management System built using **PHP** and **MySQL**, designed to manage patient records, doctor schedules, appointments, and user roles (Admin, Doctor, Patient).

---

## 📦 Prerequisites

Before you begin, ensure you have:

1. [XAMPP](https://www.apachefriends.org/index.html) installed (for Apache + MySQL)
2. A text/code editor like **VS Code**, **Notepad++**, or **Sublime Text**
3. **WinRAR** or **7-Zip** to extract zip files

---

## 📁 Installation Steps

1. **Download & Extract:**
   - Download the project ZIP: `Hospital_Management_System.zip`
   - Extract the ZIP file using WinRAR or 7-Zip

2. **Move to XAMPP Directory:**
   - Copy the extracted folder `Hospital_Management_System`
   - Paste it into your XAMPP root folder:
     ```
     C:\xampp\htdocs\
     ```

3. **Set Up the Database:**
   - Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin)
   - Create a **new database** named `hospital`
   - Click the **Import** tab
   - Select the `hospital.sql` file inside the project’s SQL folder
   - Click **Go**

4. **Run the Application:**
   - Open your browser
   - Navigate to:  
     ```
     http://localhost/Hospital_Management_System
     ```

---

## 🔐 Login Details

| Role     | Username                  | Password     |
|----------|---------------------------|--------------|
| Admin    | bensontesting@gmail.com   | programming  |
| Doctor   | totonajoyce@gmail.com     | 12345        |
| Patient  | 0725667841                | 4066         |

---

## 🧠 Features

- 🔐 Three-phase login (Admin / Doctor / Patient)
- 👨‍⚕️ Admin can manage Doctors and other Admins
- 📅 Doctor can manage patient appointments and prescriptions
- 🩺 Patient can book appointments and view reports
- 📊 Dashboard for each role
- 🛡️ Secure session-based login

---

## 🙌 Credits & Source

Developed by **Prabhu Bhalke**  
📧 Email: prabhubhalke379@gmail.com  
🌐 LinkedIn: [linkedin.com/in/prabhu-bhalke-1a258625a](https://www.linkedin.com/in/prabhu-bhalke-1a258625a/)

---

## 📌 Notes

- Ensure Apache and MySQL are running in XAMPP before starting
- Default admin is pre-loaded in the `users` table via `hospital.sql`
- You can extend functionality like email verification, password reset, or medical inventory

---

## 📧 Contact

If you face any issues or want to collaborate, feel free to connect via LinkedIn or email.
