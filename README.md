# Resource-url-routing

𝗪𝗵𝗮𝘁 𝗵𝗮𝗽𝗽𝗲𝗻𝘀 𝘄𝗵𝗲𝗻 𝘆𝗼𝘂 𝘁𝘆𝗽𝗲 𝗮 𝗨𝗥𝗟 𝗶𝗻𝘁𝗼 𝘆𝗼𝘂𝗿 𝗯𝗿𝗼𝘄𝘀𝗲𝗿?
![image](https://user-images.githubusercontent.com/41374671/212852479-e358c832-f9d9-4a4f-8f1f-0bf1aca9d57d.png)

The process involves fundamental components like browser, your computer’s operating system, your internet service provider (ISP) , the server where you host the site and the services running on that server.

𝟭.𝐘𝐨𝐮 𝐭𝐲𝐩𝐞 𝐡𝐭𝐭𝐩𝐬://𝐰𝐰𝐰.𝐭𝐡𝐞𝐭𝐫𝐚𝐢𝐧𝐥𝐢𝐧𝐞.𝐜𝐨𝐦/𝐦𝐲-𝐭𝐢𝐜𝐤𝐞𝐭𝐬 𝐢𝐧𝐭𝐨 𝐲𝐨𝐮𝐫 𝐛𝐫𝐨𝐰𝐬𝐞𝐫 𝐚𝐧𝐝 𝐞𝐧𝐭𝐞𝐫

Here, HTTPS is a scheme, which tells the browser to make a connection to the server using TLS. www.thetrainline.com is the domain name of the site and it points to a specific IP address of a server. And /my-tickets is a random path to the resource you need.

𝟮. 𝐓𝐡𝐞 𝐛𝐫𝐨𝐰𝐬𝐞𝐫 𝐜𝐡𝐞𝐜𝐤𝐬 𝐭𝐡𝐞 𝐜𝐚𝐜𝐡𝐞 𝐟𝐨𝐫 𝐚 𝐃𝐍𝐒 𝐫𝐞𝐜𝐨𝐫𝐝 𝐭𝐨 𝐟𝐢𝐧𝐝 𝐭𝐡𝐞 𝐜𝐨𝐫𝐫𝐞𝐬𝐩𝐨𝐧𝐝𝐢𝐧𝐠 𝐈𝐏 𝐚𝐝𝐝𝐫𝐞𝐬𝐬 𝐨𝐟 𝐭𝐡𝐞𝐭𝐫𝐚𝐢𝐧𝐥𝐢𝐧𝐞.𝐜𝐨𝐦/𝐦𝐲-𝐭𝐢𝐜𝐤𝐞𝐭𝐬

After you’ve typed the URL into your browser and pressed enter, the browser needs to figure out which server on the Internet to connect to. It looks for the IP address of the server hosting the website using the domain you typed to accomplish that. DNS lookup is done here. Here, it determines whether we can locate it in the cache. If not, DNS searches domain name servers from the root to the third level.

𝟯. 𝗕𝗿𝗼𝘄𝘀𝗲𝗿 𝗶𝗻𝗶𝘁𝗶𝗮𝘁𝗲𝘀 𝗧𝗖𝗣 𝗰𝗼𝗻𝗻𝗲𝗰𝘁𝗶𝗼𝗻 𝘄𝗶𝘁𝗵 𝘁𝗵𝗲 𝘀𝗲𝗿𝘃𝗲𝗿

TCP, is used throughout the public Internet routing to route packets from a client browser request through the router, the ISP, through an internet exchange to switch ISPs or networks, and finally to find the server with the IP address to connect to. This is an inefficient route to take to get there. Instead, a lot of websites utilise a CDN (like AWS CloudFront) to cache both static and dynamic material closer to the browser.

𝟰. 𝗕𝗿𝗼𝘄𝘀𝗲𝗿 𝘀𝗲𝗻𝗱𝘀 𝘁𝗵𝗲 𝗛𝗧𝗧𝗣 𝗿𝗲𝗾𝘂𝗲𝘀𝘁 𝘁𝗼 𝘁𝗵𝗲 𝘀𝗲𝗿𝘃𝗲𝗿

Now that the browser is connected to the server, it complies with the HTTP(s) protocol's requirements for communication. To request the contents of the page, the browser first sends an HTTP request to the server. The body, headers and request line of an HTTP request are all there.

𝟱. 𝗦𝗲𝗿𝘃𝗲𝗿 𝗽𝗿𝗼𝗰𝗲𝘀𝘀𝗲𝘀 𝗿𝗲𝗾𝘂𝗲𝘀𝘁 𝗮𝗻𝗱 𝘀𝗲𝗻𝗱𝘀 𝗯𝗮𝗰𝗸 𝗮 𝗿𝗲𝘀𝗽𝗼𝗻𝘀𝗲

The server accepts the request and determines how to handle it depending on the data in the request line, headers, and body. The server receives the material at this URL for the GET /page/ HTTP/1.1 requests, builds the response, and then delivers it back to the client with an HTTP status code.

𝟲. 𝗕𝗿𝗼𝘄𝘀𝗲𝗿 𝗿𝗲𝗻𝗱𝗲𝗿𝘀 𝘁𝗵𝗲 𝗰𝗼𝗻𝘁𝗲𝗻𝘁

The browser checks the response headers for instructions on how to render the resource after receiving the server's response. The Content-Type header lets the browser know that an HTML resource was received in the response body.
