
# Generate self signed SSL certificate
### (https://nodejs.org/en/knowledge/HTTP/servers/how-to-create-a-HTTPS-server/#:~:text=To%20create%20an%20HTTPS%20server%2C%20you%20need%20two%20things%3A%20an,'self%2Dsigned%20certificates'.)
> openssl genrsa -out key.pem
> openssl req -new -key key.pem -out csr.pem
> openssl x509 -req -days 9999 -in csr.pem -signkey key.pem -out cert.pem
> rm csr.pem

## Run app
> **node app.js**