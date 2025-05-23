# DHCP
**DHCP (Dynamic Host Configuration Protocol)-** is a network management protocol used to automatically assign IP addresses and other network configuration parameters (like subnet mask, gateway, and DNS) to devices on a network. It eliminates the need for manual IP configuration.



![DHCP](https://miro.medium.com/v2/resize:fit:940/1*biGJBgUqCl8OHG-_pib9VA.jpeg)

## What DHCP Does
When a device (client) connects to a network:

Requests an IP address from the DHCP server.

The DHCP server assigns an available IP from its pool.

The client uses this IP for a certain lease time.

After lease expiration, the IP can be renewed or reassigned.

## DHCP Process (DORA)
Step----------------	Message-------------------	Description
1.------------------	Discover------------------	Client broadcasts to find a DHCP server.
2. -----------------	Offer---------------------	Server responds with an available IP and configuration info.
3.------------------	Request--------------------	Client requests to use the offered IP.
4.------------------	Acknowledge----------------	Server confirms and assigns the IP to the client.

## DHCP Components
DHCP Server: Provides configuration data (IP, subnet, gateway, DNS).

DHCP Client: Device (PC, phone, printer) that receives an IP.

IP Pool: A range of IP addresses the server can assign.

Lease Time: Duration for which an IP is valid.

## Why DHCP is Important
Automates IP assignment → no need to configure each device manually.

Prevents IP conflicts → the server tracks assigned addresses.

Eases network management, especially in large or dynamic environments.

## DHCP Example
A DHCP server has a pool: 192.168.1.100 to 192.168.1.200.

When a laptop joins:

It sends a Discover.

Server Offers 192.168.1.105.

Laptop Requests 192.168.1.105.

Server Acknowledges it.

Laptop now uses 192.168.1.105 temporarily.

## DHCP Limitations / Considerations
If no DHCP server is available, clients may fail to join the network properly.

Not suitable for static devices (e.g., servers, printers) which need fixed IPs.

Rogue DHCP servers can cause network issues.

