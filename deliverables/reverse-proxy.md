# Nginx Reverse Proxy

In this setup, nginx acts as a reverse proxy between users and the Flask application.

The Flask application runs locally on port 8000 using the Gunicorn server. Users access the application through port 80, which is handled by nginx. Nginx forwards incoming HTTP requests to the Flask application running on port 8000.

Using nginx as a reverse proxy provides several benefits:

- Improved security by hiding the backend application server.
- Better performance because nginx efficiently handles many connections.
- Separation between the web server and the application server.
- Ability to scale or add additional backend services later.

This setup allows users to access the application normally through a web browser while nginx manages the communication with the Flask app.