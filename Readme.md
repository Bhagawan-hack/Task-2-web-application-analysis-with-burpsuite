 web application analysis with burpsuite

## Objective
Learn to identify and analyze potential web vulnerabilities using Burp Suite by intercepting traffic, probing manually, and automating attacks.

## Tools Used
- Burp Suite Community Edition
- Brave browser
- Foxyproxy(extension)
- Custom Wordlist
  

### 1. Installation
### 2. Proxy Configuration
### 3. Certificate Setup
### 4. Intercepting Request
### 5. Manual Testing with Repeater
### 6. Automated Attack with Intruder
### 7. Results and Comparison


### 1. Installation

#### Step 1 — Check Java

First, check if Java is installed on your system. Java is required to run Burp Suite.

**To check Java:**
Open Command Prompt and run:

```
java -version
```

If the command displays a Java version, Java is already installed. If not, download and install Java from: [https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/)

![java](https://github.com/user-attachments/assets/95b5327f-5a55-40a8-b367-52d7e32a85a1)

![download java](https://github.com/user-attachments/assets/0ce62843-3771-44c8-a2c9-6f1e574520ed)
Select your PC's bit version and start the download.

#### Step 2 — Install Burp Suite

To download Burp Suite Community Edition, visit: [https://portswigger.net/burp/communitydownload](https://portswigger.net/burp/communitydownload)

![burpsuite](https://github.com/user-attachments/assets/6bcbfec0-f049-4feb-91c7-fe485b19d108)

### 2. Proxy Configuration

#### Step 1 — Install FoxyProxy

Download the FoxyProxy extension for your browser:
[https://chromewebstore.google.com/detail/foxyproxy/gcknhkkoolaabfmlnjonogaaifnjlfnp?hl=en](https://chromewebstore.google.com/detail/foxyproxy/gcknhkkoolaabfmlnjonogaaifnjlfnp?hl=en)

![proxy](https://github.com/user-attachments/assets/cc016a39-afcc-4519-9574-1477a8a84018)

#### Step 2 — Configure the proxy

Open the FoxyProxy extension and add a new proxy with the following settings:

* **Title:** task 2
* **Hostname:** 127.0.0.1
* **Port:** 8080

![setup](https://github.com/user-attachments/assets/33444a26-323e-4f4d-aa83-106400552015)

### 3. Certificate Setup

1. In your browser, go to: `http://burp`.
2. Download the **CA Certificate** from the page.
3. Open your browser settings and navigate to **Manage Certificates** (or **Certificates** → **Import** in Windows).
4. Import the downloaded Burp CA certificate into the **Trusted Root Certification Authorities** (or the equivalent store for your browser).
5. Restart your browser to apply the changes.

![step 1](https://github.com/user-attachments/assets/5b69f63f-b9c6-473e-bf7a-1b866012794c)
*Import the certificate from here into your browser.*



