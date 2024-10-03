# Internet & Web Protocols (HTTP/HTTPS, DNS)

## 1. **HTTP (Hypertext Transfer Protocol)**

![image](https://github.com/user-attachments/assets/664209b0-e69d-4bad-abbc-ef240698e79a)

### Overview:
HTTP is a communication protocol used to send and receive data between a client (browser) and a server over the World Wide Web. HTTP operates under a **client-server** model, where the browser acts as the client making a request, and the server responds to the request.

### Characteristics of HTTP:
- **Stateless**: Each HTTP request is independent; there is no connection between one request and another.
- **Methods**: HTTP has various methods like:
  - **GET**: Retrieves data from the server.
  - **POST**: Sends data to the server.
  - **PUT**: Updates data on the server.
  - **DELETE**: Deletes data on the server.
- **Status Codes**: The server responds with a status code to indicate the outcome of the request, examples include:
  - **200 OK**: The request was successful.
  - **404 Not Found**: The resource could not be found.
  - **500 Internal Server Error**: There was an error on the server.

### HTTP Workflow:
1. The client sends an HTTP request (e.g., asking for a web page).
2. The server receives the request, processes it, and sends back an HTTP response (e.g., delivering the requested web page).

## 2. **HTTPS (Hypertext Transfer Protocol Secure)**

![image](https://github.com/user-attachments/assets/ab7f6995-5199-44c4-8b06-07e5bc628a11)

### Overview:
HTTPS is the secure version of HTTP, using SSL/TLS encryption to protect the data being transmitted between the client and server. This is important for ensuring the privacy and integrity of data, especially on websites that handle sensitive information like passwords or credit card details.

### Advantages of HTTPS:
- **Data Security**: All data sent over HTTPS is encrypted, meaning only the intended parties can read it.
- **Data Integrity**: HTTPS prevents data from being tampered with during transmission.
- **Authentication**: SSL/TLS certificates verify that the server you are connecting to is legitimate.

### HTTPS Workflow:
1. The client connects to the server over HTTPS.
2. The SSL/TLS handshake process begins to establish a secure session.
3. Data is encrypted and transmitted securely between the client and server.

## 3. **DNS (Domain Name System)**

![image](https://github.com/user-attachments/assets/81e4b7e8-5251-431b-998e-021846ba02e0)

### Overview:
DNS is a system that translates easy-to-remember domain names (like `www.example.com`) into numeric IP addresses (like `192.0.2.1`) used by computers to communicate with each other over a network.

### DNS Components:
- **Domain**: A unique name used to identify a website.
- **Nameservers**: Servers responsible for answering DNS queries and providing the IP address that corresponds to the domain name.
- **Zone File**: Contains DNS records for a specific domain, including IP addresses linked to subdomains and other services.

### Types of DNS Records:
- **A Record**: Maps a domain name to an IPv4 address.
- **AAAA Record**: Maps a domain name to an IPv6 address.
- **CNAME Record**: Redirects one domain to another domain.
- **MX Record**: Specifies the email server used by the domain.

### DNS Workflow:
1. The browser requests the IP address for a specific domain.
2. The DNS resolver checks its cache; if not found, it queries a DNS server.
3. The DNS server responds with the IP address for the domain.
4. The browser uses the IP address to connect to the server and retrieve data (e.g., a web page).
