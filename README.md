# Pi-hole DNS Filtering with Raspberry Pi

![Pi-hole Dashboard](https://github.com/user-attachments/assets/sampleimg1)

## Objective
This project involved setting up a Raspberry Pi as a DNS server with **Pi-hole** to filter network traffic, block ads, and enhance security. The goal was to provide DNS-based filtering for all devices on the local network by routing their DNS queries through Pi-hole.

### Skills Learned
- Raspberry Pi setup and configuration.
- Installation and configuration of Pi-hole for DNS filtering.
- Network troubleshooting and management.
- Using static IP addresses for network stability.
- Managing DNS queries and monitoring network traffic.

### Tools Used
- **Raspberry Pi 4**: Hardware for hosting Pi-hole.
- **Micro SD Card**: Storage for the Raspberry Pi OS.
- **Pi-hole**: DNS filtering tool.
- **SSH**: For remote access to the Raspberry Pi.
- **Router**: For configuring static IP and DNS settings.
- **Web-based Pi-hole Admin Interface**: For managing DNS traffic.

## Steps

### Step 1: Raspberry Pi Setup
Connected the Raspberry Pi to power and network, and installed Raspberry Pi OS on a micro SD card using the Raspberry Pi Imager tool. Powered it on and completed the initial setup via SSH.

*Ref 1: Raspberry Pi Setup*

![Raspberry Pi Setup](https://github.com/user-attachments/assets/sampleimg2)

### Step 2: Static IP Configuration
Set a static IP for the Raspberry Pi to ensure it remains accessible within the network. This step involved editing the DHCP settings on the router or configuring static IP within the Pi's network settings.

*Ref 2: Static IP Setup*

![Static IP Configuration](https://github.com/user-attachments/assets/sampleimg3)

### Step 3: Pi-hole Installation
Installed Pi-hole by running the installation script from the Pi-hole website. Configured Pi-hole to function as the primary DNS server for the network, filtering unwanted ads and malicious domains.

*Ref 3: Pi-hole Installation Process*

```bash
curl -sSL https://install.pi-hole.net | bash
```

### Step 4: Device DNS Setup
Changed the DNS settings on individual devices (phones, computers, etc.) to point to the static IP of the Raspberry Pi, ensuring that all DNS traffic routes through Pi-hole for filtering.

*Ref 4: Device DNS Configuration*

![Device DNS Setup](https://github.com/user-attachments/assets/sampleimg5)

### Step 5: Monitoring and Configuration
Used the Pi-hole admin interface to monitor DNS queries, review blocked domains, and adjust filtering rules as needed. Custom configurations included whitelisting essential domains and further tweaking DNS settings.

*Ref 5: Pi-hole Admin Interface*

![Pi-hole Admin Dashboard](https://github.com/user-attachments/assets/sampleimg6)

## Conclusion
This project provided valuable experience in configuring a Raspberry Pi as a DNS filtering server using Pi-hole. The setup improved network security and privacy by blocking ads and malicious domains, while offering real-time monitoring of network traffic through the Pi-hole dashboard.
