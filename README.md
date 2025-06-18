# Nameserver IP checker

Sure! Here's a clean and concise **README summary** section you can add to your GitHub project:

---

### 🧾 Nameserver IP Checker (Python)

This simple Python script uses the `socket` module to resolve and display the IP addresses of given **DNS nameservers**.

#### ✅ Features:

* Converts nameservers (e.g. `ns1.shopify.com`) to their corresponding IP addresses.
* Useful for DNS diagnostics, registrar systems, or validating glue records.

#### 🧪 Example Output:

```bash
IP address of ns1.shopify.com is 23.227.38.65  
IP address of ns2.shopify.com is 23.227.38.65  
IP address of ns-cloud-a1.googledomains.com is 216.239.32.106  
IP address of ns1.bluehost.com is 162.88.60.37  
```

#### 🐍 How to Use:

1. Make sure you have Python installed.
2. Run the script:

   ```bash
   python nameserver_ip_checker.py
   ```

#### 🛠 Code Overview:

```python
import socket

nameserver1 = 'ns1.shopify.com'
nameserver2 = 'ns2.shopify.com'
nameserver3 = 'ns-cloud-a1.googledomains.com'
nameserver4 = 'ns1.bluehost.com'

ip_address1 = socket.gethostbyname(nameserver1)
ip_address2 = socket.gethostbyname(nameserver2)
ip_address3 = socket.gethostbyname(nameserver3)
ip_address4 = socket.gethostbyname(nameserver4)

print(f"IP address of {nameserver1} is {ip_address1}")
print(f"IP address of {nameserver2} is {ip_address2}")
print(f"IP address of {nameserver3} is {ip_address3}")
print(f"IP address of {nameserver4} is {ip_address4}")
```

---

Let me know if you'd like to extend it to check more nameservers or add exception handling!
