# node-sample-app
An instructional sample application that details how to access Citi's Accounts API through 3-legged OAuth. For more details on Citi's APIs, visit developer.citi.com.
To successfully run the application:
Running the application:

1. Register for a Citi Developer Hub Account.

2. Login to the Citi Developer Hub.

3. Create a new application. 3a. enter 'https://127.0.0.1:3000/accounts/retrieve' as your redirect URI. Write down your client id and client secret (CLIENT_ID, CLIENT_SECRET).

4. Create a new folder for your sample application.

5. Install or ensure that you have the latest versions of Node (https://nodejs.org) and OpenSSL (https://openssl.org).

6. Using OpenSSL in your new folder, execute the following command: openssl req -x509 -newkey rsa:2048 -keyout key.pem -out cert.pem -days 365. Write down whatever password you create (CERTIFICATE_PASSWORD). For COMMON NAME, put 'localhost'. Verify that key.pem and cert.pem exist in your new folder.

7. Place package.json, index.html, and server.js in your new folder either through direct download or git.

8. Enter your application credentials into config.json and login.html. CLIENT_ID, CLIENT_SECRET, and CERTIFICATE_PASSWORD are what were copied above - enter them into config.json. In login.html - replace <REPLACE WITH YOUR APPLICATION'S CLIENT ID> with your CLIENT_ID.

9. in your new folder, run the following command: node server.js

10. You should get a confirmation the server is running on port 3000.

11. Navigate to https://127.0.0.1:3000 on your browser. accept the self-signed certificate, and follow the onscreen prompts to test your application.
