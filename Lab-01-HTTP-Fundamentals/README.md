# Objective

The purpose of this lab is to understand the basics of the Hypertext Transfer Protocol (HTTP), compare it with HTTPS, identify common HTTP status codes, and observe a real HTTP request using the browser's Developer Tools.

## HTTP

HTTP (Hypertext Transfer Protocol) is a protocol that allows a web browser to communicate with a web server. Whenever a user visits a website, the browser sends an HTTP request to the server, and the server responds with the requested resources such as HTML pages, images, CSS, JavaScript files or other content.

HTTP transfers data in plain text in not encrypted form during transmission. Because of this, anyone who intercepts the traffic can potentially read or modify the data.

## Difference Between HTTP and HTTPS

| HTTP | HTTPS |
| :--- | :--- |
| Stands for Hypertext Transfer Protocol | Stands for Hypertext Transfer Protocol Secure |
| Data is transmitted in plain text | Data is encrypted using TLS (Transport Layer Security) |
| No encryption or authentication | Provides encryption, authentication, and data integrity |
| Uses Port 80 | Uses Port 443 |
| Less secure beacause of plain text communication | Much more secure than HTTP |

## HTTPS is More Secure

because it protects data by encrypting the communication between the browser and server. If an attacker captures the network traffic, communication appear as encrypted data rather than readable information such as usernames, passwords, or cookies.

## Common HTTP Status Codes

| Status Code | Meaning |
| :--- | :--- |
| 200 OK | Success (The server successfully processed the request.) |
| 301 Moved Permanently | Permanent Redirect (The requested resource has permanently moved to a new URL.) |
| 302 Found | Temporary Redirect (The resource is temporarily located at another URL.) |
| 403 Forbidden | Access Denied (The server understood the request but refuses to authorize it.) |
| 500 Internal Server error | Server Error (The server encountered an unexpected error while processing the request.) |

## Request Analysis

During this lab, I searched for TryHackMe login in Google while monitoring the browser's Network tab.

The first request shown in the Network tab is a GET request sent from my browser to www.google.com. The server successfully processed the request and returned an HTTP 200 (OK) response, indicating that the search resuls page was loaded successfully.

After the initial page was loaded, the browser automatically made several additional requests to download supporting resources. These additional requests are required for the webpage to display and function correctly.

The browser also received 301 and 302 redirect responses for some resources. These redirects instruct the browser to request the resource from a different location before continuing to load the webpage.

This observation shows that loading a modern website is not a single request. The browser sends many HTTP requests to retrieve all the resources required to fully render the page.

## What I Learned

- HTTP is the protocol used for communication between web browsers and web servers.
- HTTP sends data in plain text, making it vulnerable to interception.
- HTTPS encrypts communication using TLS to protect sensitive information.
- HTTP status codes indicate whether a request was successful or if an error occurred.
- The browser's Network tab is useful for analyzing HTTP requests and understanding how websites load resources.
