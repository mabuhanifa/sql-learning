To configure and start **MySQL** and **MySQL Workbench** on **Ubuntu**, follow these steps:

---

### 🧱 1. **Install MySQL Server**

Open a terminal and run:

```bash
sudo apt update
sudo apt install mysql-server
```

After installation, check if MySQL is running:

```bash
sudo systemctl status mysql
```

✅ If it's inactive, start it:

```bash
sudo systemctl start mysql
```

And enable it to start on boot:

```bash
sudo systemctl enable mysql
```

---

### 🔐 2. **Secure MySQL Installation**

This will guide you through setting root password, removing test users, etc.:

```bash
sudo mysql_secure_installation
```

Follow the prompts to:

- Set a root password
- Remove anonymous users
- Disallow remote root login
- Remove test database
- Reload privilege tables

---

### 🔑 3. **Login to MySQL**

```bash
sudo mysql -u root -p
```

If you're using **auth_socket** plugin (common in Ubuntu), and want to use password-based login:

```sql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'your_password';
FLUSH PRIVILEGES;
EXIT;
```

---

### 🧰 4. **Install MySQL Workbench**

```bash
sudo apt install mysql-workbench
```

If it's not available from apt or outdated, use snap:

```bash
sudo snap install mysql-workbench-community
```

Or download from [MySQL official site](https://dev.mysql.com/downloads/workbench/).

---

### 🚀 5. **Start MySQL Workbench**

Run from terminal:

```bash
mysql-workbench
```

Or find it in your application menu.

---

### 🧷 6. **Connect to MySQL from Workbench**

1. Open MySQL Workbench
2. Click the `+` icon next to **MySQL Connections**
3. Set:
   - Connection Name: Anything
   - Hostname: `127.0.0.1` or `localhost`
   - Port: `3306` (default)
   - Username: `root` (or your MySQL user)
4. Click **Store in Vault** to save password
5. Click **Test Connection** → then **OK**

---

Let me know if you run into any issues — I can help troubleshoot errors too.

To create a **database called `movieDB`** in MySQL, follow these steps:

---

### 📌 Option 1: Using MySQL CLI

1. Open terminal:

```bash
mysql -u root -p
```

2. Once inside the MySQL shell, run:

```sql
CREATE DATABASE movieDB;
```

3. To check if it was created:

```sql
SHOW DATABASES;
```

4. To use it:

```sql
USE movieDB;
```

5. Then you can start creating tables, e.g.:

```sql
CREATE TABLE movies (
  id INT AUTO_INCREMENT PRIMARY KEY,
  title VARCHAR(255),
  release_year INT
);
```

---

### 📌 Option 2: Using MySQL Workbench

1. Open MySQL Workbench
2. Connect to your MySQL server (local or remote)
3. In the **Navigator** panel on the left:
   - Right-click **Schemas**
   - Choose **Create Schema**
4. In the popup:
   - **Name**: `movieDB`
   - Click **Apply**, then **Apply** again to execute the SQL
   - Click **Finish**

You’ll now see `movieDB` listed under **Schemas**. Right-click and set it as default if you want to work within it.

---

Let me know if you'd like help creating tables or inserting sample data into `movieDB`.
