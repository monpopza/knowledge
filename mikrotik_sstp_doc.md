[Back](https://github.com/monpopza/knowledge) | [Home](https://github.com/monpopza)

# Mikrotik CHR How to create vpn SSTP
## [Document](https://mum.mikrotik.com/presentations/ME16/presentation_3821_1476714592.pdf)
## Step to Step
### Setting Timezone
- System/Clock/Set time

### Update Time with SNTP Link
- System/SNTP Client 
  - Enable 
  - Primary:time.apple.com 
  - Secondary: time.windows.com (EZ)
- Click Apply and OK

### Generate Certificate 
- System/Certificate 
- Click (+) with 2 Windows
  - Windows 1: General
    - Name:CA
    - Country:NA
    - (ALL:NA Until Unit)
    - Common Name: URL 
    - (NOTE: not IP address with DDNS IP if have DDNS Service Use DDNS SERVICE)
    - Days Valid: 3650
  - Windows 1: Key Usage
    - Uncheck All Box Check
    - Checked: CRL SIGN | Ket Cert. sign
    - Click Apply to saved

  - Windows 2: General
    - Name:Server
    - Country:NA
    - (ALL:NA Until Unit)
    - Common Name: URL 
    - (NOTE: not IP address with DDNS IP if have DDNS Service Use DDNS SERVICE)
    - Days Valid: 3650
  - Windows 2: Key Usage
    - Uncheck All Box Check
    - Click Apply to saved

### Signing Certificates
- Windows CA
  - Click Sign 
    - Certificate: CA
    - CA: None/Blank
    - Click Sign
    - and close window
- Wuindows Server
  - Click Sign 
    - Certificate: Server
    - CA: CA
    - Click Sign
    - and close window

### Export Certificate
- Right Click CA Certificate
  - Export
  - Certificate > CA
  - Export
  - Close

## IP VPN Setting
### ADD IP to IP POOL
- IP/Pool
  - Click (+)
  - NAME: SSTP_IP
  - Address: As your wish (Range of IP) 
  - (NOTE: 192.168.1.2-192.168.1.22
  - Clock Apply

### PPP Profile
- PPP
  - Profile Tab
  - Click (+)
    - General
      - NAME: SSTP Profile
      - > Local Address: (Your router IP in VPN)
      - (NOTE: 192.168.1.1)
      - Remote Access: SSTP_IP (from pool)
      - DNS: Your Provider or Router IP DNS
    - Protocols
      - USE MPLS: Def
      - ComL Def
      - Encrypt: YES
      - Click Apply and OK

  - Secret Tab
  - Click (+)
    - NAME: Your ID
    - Pass: Your Pass
    - Service: any
    - Profile: SSTP Profile
    - Click Apply and OK

  - Interface Tab
  - SSTP Server
    - Enable: Yes
    - Defalut ProfileL SSTP Profile
    - Authentication: mschap2 only
    - Certificate: Server
    - TLS: any
    - Verify: No 
    - Click Apply and OK

### DOWNLOAD CRT AND INSTALL
- GOTO FILE
- DRAG AND DROP TO YOUR DESKTOP OR RIGHT CLICK TO DOWNLOAD AND INSTALL IT
- INSTALL WITH TRUST ROOT CERTIFICATE 
  - LOCAL MACHIN/TRUSTED ROOT CERTIFICATE  

[Back](https://github.com/monpopza/knowledge) | [Home](https://github.com/monpopza)
