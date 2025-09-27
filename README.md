## 1. simple_auth source code
a. basic_auth.js
Bước 1: Run the server

Bước 2: Open Postman and create a GET request to:
2.1 `http://localhost:3000`
- Go to the Authorization tab, select Basic Auth
- Enter: Username: `admin`, Password: `12345`
- Send the request.
- Check the response (e.g., 200 OK with "welcome" message).
- results: "Welcome! Visit first public resource."
- ![Basic Auth Test](simple_auth/public/results/basic_auth2.png)
2.2 `http://localhost:3000/secure`
- Go to the Authorization tab, select Basic Auth
- Enter: Username: `admin`, Password: `12345`
- Send the request.
- Check the response (e.g., 200 OK with "welcome" message).
- results: "You have accessed a protected resource 🎉"
- ![Basic Auth Test](simple_auth/public/results/basic_auth1.png)
2.3 `http://localhost:3000/public`
- Go to the Authorization tab, select Basic Auth
- Enter: Username: `admin`, Password: `12345`
- Send the request.
- Check the response (e.g., 200 OK with "welcome" message).
- results: "Welcome! Visit second public resource."
- ![Basic Auth Test](simple_auth/public/results/basic_auth3.png)

## 2. cookie_auth.js
Bước 1: Run the server

Bước 2: Open Postman and create a POST request to:
- select body, select raw
- Enter: {Username: `admin`, Password: `12345`}
- Send the request.
- Check the response (e.g., 200 OK with "welcome" message).
- results: "Logged in!"
- ![Cookie Auth 1](simple_auth/public/results/cookie_auth1.png)

Bước 3: open MongoDB Compass
Bước 4: connect localhost
bước 5: select database cookieApp
bước 6: select collection cookies
- ![Cookie Auth 2](simple_auth/public/results/cookie_auth2.png)


