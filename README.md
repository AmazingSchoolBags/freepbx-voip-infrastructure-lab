# FreePBX VoIP Infrastructure Lab

Design and deployment of a professional VoIP infrastructure using **Asterisk / FreePBX**.

This lab simulates a small enterprise telephony system with multiple services, call routing and security mechanisms.

## Architecture

The platform was deployed on a Debian server with FreePBX and includes:

- SIP extensions
- IVR (Interactive Voice Response)
- Ring groups
- Call queues
- Time conditions (business hours / lunch break)
- Emergency mode (Call Flow Control)
- Call parking
- Conferences
- Follow-me call routing

## Security

The infrastructure was hardened with:

- **UFW Firewall**
- Restricted access to internal networks  
  `172.19.0.0/16`  
  `192.168.1.0/24`

Allowed services:

- SSH
- HTTP (FreePBX interface)
- SIP
- RTP

Protection against attacks implemented with:

- **Fail2Ban**
- SSH brute-force protection
- SIP attack detection and automatic IP banning

## Tests performed

The following tests were validated:

- Internal SIP calls
- IVR routing
- Queue call distribution
- Business hours routing
- Lunch break routing
- Emergency call mode
- Call parking
- Follow-me functionality
- Firewall filtering
- SIP brute-force detection with Fail2Ban

## Technologies used

- Asterisk
- FreePBX
- SIP / RTP
- UFW Firewall
- Fail2Ban
- Debian Linux

## Documentation

Full project documentation is available here:

📄 **FreePBX_VoIP_Infrastructure_Lab.pdf**

---

VoIP infrastructure lab project developed as part of a network and system administration training.
