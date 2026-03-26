# Packet-Tracer-Star-Topology


# Overview 

Star Topology is kind of like the airport (switch); there are many different airlines. Many planes (computers) go to different destinations (packets). But every plane has to land within that airport to refuel, gather people, etc. Everything goes through the middle, and then out to the destination, which is Star topology; all devices connect to one central device. 


Star topology is the go-to choice in real networks. If one device breaks, nobody else suffers if PC 2 completely dies or gets unplugged; every other computer on the network keeps working perfectly, so that one problem stays isolated. The second reason is that it is super easy to troubleshoot. It's easy to add new devices by just plugging a device into an open port on the switch and configuring it, and I wouldn't have to touch or reconfigure anything else in the network. It's also very easy to remove devices without disrupting anything within the network. If someone just leaves the company, I can just remove the computer by unplugging it, and nobody else on the network will feel it at all. 

1. Now, I opened up Cisco Packet Tracer and started with a new project, and I will drag in five PCs and one switch to the table. 

<img width="732" height="548" alt="image" src="https://github.com/user-attachments/assets/cb24b8f8-88dd-4723-a9a0-b5ac0e00ba5f" />

2. I will connect each computer to the switch and then assign a static IP address to each device. Now, a switch is my central point, kinda like the post office. Every letter, which is the data from every house, which is the PC, goes to the post office first, and then the post office figures out where the data will be delivered.

<img width="1360" height="873" alt="image" src="https://github.com/user-attachments/assets/5657f421-ead4-4840-94d8-fb2ccaf7226c" />


3. I will assign each IP Address below.

PC0: 192.168.1.10
PC1: 192.168.1.11
PC2: 192.168.1.12
PC3: 192.168.1.13
PC4: 192.168.1.14

<img width="757" height="525" alt="image" src="https://github.com/user-attachments/assets/a42d24ec-9de7-4549-ae5d-c91369030f3c" />

<img width="820" height="571" alt="image" src="https://github.com/user-attachments/assets/5308128b-b528-4e01-9895-0cf6191d8158" />

4. After setting all computers with a static IP address, I will now test by pinging another computer using the CLI. I will go to PC0 CLI and ping PC4 with the IP Address 192.168.1.14 and follow the data being transmitted.

Basically, I am testing the connection with a ping that is like a sonar in a submarine or a game that people play called Marco Polo. I'm sending a digital hello, which is an ICMP request to PC4, and I'm waiting for PC4 to yell back I'm here.


<img width="1068" height="594" alt="image" src="https://github.com/user-attachments/assets/56abba46-ae97-4811-afc6-61fbea4d8e9f" />

It sent out 4 packets and was able to receive 4 packets. This was successful.

<img width="1392" height="642" alt="image" src="https://github.com/user-attachments/assets/2a7d52a8-2c6a-4ab2-b4b9-ccf52f9274f3" />


# Final Thoughts

I use static IPs to understand the foundation, and in a real enterprise environment, I would implement DHCP. It prevents IP conflicts when two people are trying to use the same address and saves hundreds of hours of manual labor as the company grows. DHCP will give an available IP address automatically, depending on whether the device stays on the network for either 24 hours or forever.

The switch is like the Death Star exhaust for the one single point of failure that can take down the whole station if it's not protected.
