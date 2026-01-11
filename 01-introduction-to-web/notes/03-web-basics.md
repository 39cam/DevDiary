# Basic Preparation: Web Basics

> **Disclaimer:**  
> These notes reflect my personal understanding of how the web works.  
> They are written for learning purposes and do not reproduce any proprietary course material.

---

## 1. What Is the Internet?

The **internet** is a global network of interconnected computers.  
Its main purpose is to allow devices to communicate with each other, regardless of physical distance.

This global connection is made possible through:
- Submarine fiber-optic cables
- Terrestrial fiber networks
- Satellites
- Routers and data centers distributed around the world

At its core, the internet is the **infrastructure** that enables communication.  
The **web** is a service built on top of that infrastructure.

---

## 2. How Data Travels Across the Internet

When you request information (for example, opening a website), the data does not travel as a single piece. Instead, it is broken into **small units called packets**.

### General Flow

1. A request is sent from your device (client)
2. The request travels through your Internet Service Provider (ISP)
3. Routers forward packets across different networks
4. The request reaches the destination server
5. The server sends packets back to your device
6. Your device reassembles the packets into usable data

Routers ensure packets can find alternative paths if part of the network is unavailable, making the internet resilient.

---

## 3. Internet vs Web

- **Internet:**  
  The technical infrastructure that connects computers worldwide.

- **World Wide Web (Web):**  
  A service that uses the internet to deliver documents, images, and applications through browsers.

The web relies on the internet, but the internet can exist without the web.

---

## 4. Clients, Servers, and ISPs

### Client
A **client** is a device (computer, phone, tablet) that:
- Is connected to the internet through an ISP
- Requests data from servers
- Commonly uses a web browser

### Server
A **server** is a computer that:
- Is directly connected to the internet
- Stores websites, applications, or data
- Responds to client requests

A single server can host multiple websites.

### Internet Service Provider (ISP)
An **ISP** connects client devices to the internet and assigns them IP addresses.

---

## 5. IP Addresses and DNS

### IP Address
An **IP address** (Internet Protocol address) is a unique identifier assigned to each device connected to the internet.  
It allows devices to locate and communicate with each other.

### Domain Names and DNS
Humans use **domain names**, while computers use IP addresses.

The **Domain Name System (DNS)** acts like an address book:

1. You enter a domain name (e.g. `example.com`)
2. The browser queries a DNS server
3. The DNS server returns the IP address
4. The browser sends a request to the correct server

---

## 6. Data Centers and Physical Infrastructure

Web servers are usually located inside **data centers**, which store large amounts of data and computing resources.

Data transmission primarily occurs through **fiber-optic cables**, where data travels as pulses of light.  
Wireless technologies (Wi-Fi, cellular networks) still rely on these cables at some point in the communication path.

---

## 7. Protocols and Communication Rules

A **protocol** defines rules for data transmission and communication between devices.

Common protocols include:
- **IP (Internet Protocol):** Addressing and routing
- **TCP:** Reliable data transfer
- **HTTP / HTTPS:** Web communication

Protocols ensure that devices understand each other.

---

## 8. Web Pages, Websites, and Related Concepts

### Web Page
A **web page** is a document displayed in a web browser.  
It is typically written in **HTML**.

### Website
A **website** is a collection of related web pages under a single domain name.

### Web Server
A **web server** is a computer that hosts websites and makes them accessible over the internet.

### Web Application
A **web application** is software that runs on a server and responds to client requests to perform actions or provide data.

### Web Browser
A **web browser** is a client application used to request, receive, and display web content.

### Search Engine
A **search engine** is a web service that helps users find web pages.  
Examples include Google, Bing, and DuckDuckGo.

---

## 9. Intranets and Extranets

- **Intranet:**  
  A private network accessible only within an organization.

- **Extranet:**  
  A private network that grants limited access to external partners or organizations.

---

## 10. HTTP and the Request–Response Cycle

Web communication is based on the **request–response model**, primarily using **HTTP (Hypertext Transfer Protocol)**.

### Example Flow

1. The browser sends an HTTP request (e.g. `GET`)
2. The server processes the request
3. The server sends an HTTP response
4. The browser receives and processes the response

### Loading a Web Page

- The browser first requests the main HTML file
- The HTML file references other resources (CSS, JavaScript, images)
- The browser sends additional requests for those resources
- Once all resources are received, the browser renders the page

---

## References

The following resources were used as **conceptual learning material** to understand how the internet and the web work.  

### Articles & Documentation
- MDN Web Docs – *How does the Internet work?*  
  https://developer.mozilla.org/en-US/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work

- MDN Web Docs – *Browsing the Web*  
  https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Environment_setup/Browsing_the_web

- MDN Web Docs – *How the Web works (Clients and Servers)*  
  https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Web_standards/How_the_web_works#Clients_and_servers

- MDN Web Docs – *What is a Domain Name?*  
  https://developer.mozilla.org/en-US/docs/Learn_web_development/Howto/Web_mechanics/What_is_a_domain_name#how_does_a_dns_request_work

### Videos
- *How the Internet Works* – YouTube  
  https://www.youtube.com/watch?v=eHp1l73ztB8

- *How the Web Works* – YouTube  
  https://www.youtube.com/watch?v=7_LPdttKXPc

## Final Notes

Understanding how the web works at a high level is essential before learning web development.  
