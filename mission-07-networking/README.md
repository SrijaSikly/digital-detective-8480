# Mission 7 — How computers communicate

## 1. Task / objective
The task was to explain basic network types and concepts, observe connectivity and DNS lookup information using Terminal, and describe what happens when a website opens.

## 2. Work completed

### Task 7.1 — Network concepts

| Concept | Explain it in your own words | Example |
|---------|------------------------------|---------|
| LAN | A network that covers a small area, so devices close together can share data and resources | The Wi-Fi network in a home or a college lab |
| MAN | A network that covers a whole city or a large campus, joining several LANs | A university network linking all its campus buildings |
| WAN | A network that covers a very large area, even across countries | The internet |
| DNS | A system that turns a domain name that people remember into the IP address that computers use | Turning example.com into its IP address |
| Router | A device that connects networks and decides where to send data next | The home Wi-Fi router connecting my laptop to the internet |
| Protocol | A set of rules that devices follow so they can understand each other | HTTP and HTTPS for websites |
| Packet switching | Data is cut into small packets that travel separately and are put back together at the destination | A photo sent online arrives as many packets |
| Client-server | A client asks for a service and a server provides it | My browser (client) requesting a web page from a web server |

### Task 7.2 — Network observations
I ran `ping -c 4 example.com` and `nslookup example.com`.

- `ping` result: 4 packets sent, 4 received, 0% packet loss, with an average reply time of about 10 ms.
- `nslookup` result: example.com has the IP addresses 172.66.147.243 and 104.20.23.154. I did not record my own network's details.

Answers:
- **What a connectivity test helps me check:** whether my computer can reach another computer over the network, whether the replies come back (packet loss), and how long they take.
- **What a DNS lookup displays:** the IP address (or addresses) linked to a domain name, and which DNS server answered.
- **Role of DNS when I type a website name:** the browser cannot connect using a name, so DNS first finds the IP address for that name. Then the browser can connect to that address.

### Task 7.3 — What happens when I open a website
1. I type a website address in my browser, which acts as the **client**.
2. The browser asks **DNS** to find the IP address that belongs to the domain name.
3. DNS replies with the IP address of the server.
4. The browser sends a request, using a **protocol** such as HTTPS, from my computer through my router and across the internet. The request is split into packets.
5. The packets travel through several routers until they reach the web **server**.
6. The server finds the page and sends back a response, as packets, over the same kind of path.
7. My browser puts the packets together and displays the web page on my screen.

## 3. Commands / tools used
- `ping -c 4 example.com`: tests whether a public website can be reached and how fast it replies.
- `nslookup example.com`: does a DNS lookup to find the IP address of a domain.
- VS Code: used to write the README.
- Git: `git add`, `git commit`, `git push` to save the mission.

## 4. My understanding
A network lets devices exchange data. LAN, MAN and WAN differ by the area they cover. DNS works like a phone book for the internet, turning names into IP addresses. Routers pass packets between networks, and protocols are the rules that make communication possible. When I open a website, my browser (client) uses DNS to find the server, sends a request in packets, and the server sends back the page.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-07-networking/README.md`

No raw terminal output was added, to keep my network details private.

## 8. Commit details
Commit message: "Explain networking concepts and website communication"

The work was pushed to GitHub and I confirmed the file and commit are visible.