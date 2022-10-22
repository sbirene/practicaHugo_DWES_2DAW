---
weight: 3
bookFlatSection: true
title: "Client --> Server"
---

# Communication of a client with a server

On this page we will try to explain the process by which a client communicates with a server.

The *client-server architecture* or *client-server model* is a communication protocol through a network (such as the Internet) in which the tasks are distributed among the providers of resources or services, called **servers**, and the plaintiffs, called **clients**.

A client makes requests to another program, the server, which responds.

In this case, to explain how communication is carried out, we are going to focus on the process of loading a web page.

It is important to mention that a large part of Internet services obey the *client-server architecture*. The web server makes the websites available to the client, which are accessed through the browser. It is the server that hosts the data that the client (browser) requests.

### Important concepts:
>> **Client**: device connected to the Internet (for example, a computer connected to the Wi-Fi network or a phone connected to the mobile phone network) and the software that is available and allows access to the Internet (usually , a web browser).

>> **Server**: computer that stores web pages, sites or applications.

>> **TCP/IP: Transmission Control Protocol and Internet Protocol**, communication protocols that define how data should travel through the web.

>> **DNS**: servers of the **Domain Name System**, we could define them as a website address book. When you type a web address into your browser, usually a domain (such as *www.google.es*), DNS translates that domain name to its IP address to find out which server the website lives on so it can send HTTP messages to correct place.

>> **HTTP**: Hypertext Transfer Protocol, is an application protocol that defines how clients and servers communicate.

## What happens then?
When you type a web address (or domain) in the browser:

1. The browser goes to the DNS server and finds the real address of the server where the website is hosted.
2. The browser sends an HTTP request message to the server, asking it to send a copy of the web page to the client. This message, and all data sent between the client and the server, is sent over the Internet connection using TCP/IP.
3. Whenever the server approves the client's request, the server will start sending the web page files to the browser as a series of small chunks called data packets.
4. The browser puts the little pieces together, forms a complete website and shows it to you.

## Graphic example

{{< mermaid>}}
flowchart LR
    id1(Client - Browser)-->id2(DNS)
    id2-- IP adress -->id1
    id1-->id3{{Internet}}-->id4[(Server)]
{{< /mermaid >}}

Once the request is approved:
{{< mermaid>}}
flowchart LR
    id4[(Server)]-->id3{{Internet}}-->id1(Client - Browser)
{{< /mermaid >}}