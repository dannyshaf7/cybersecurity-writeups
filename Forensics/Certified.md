Certified from US Cyber Games Summer 2024
Author: tsuto

<img width="504" alt="image" src="https://github.com/user-attachments/assets/fc091533-298c-4330-b3eb-beb2ec525ad3">

Source 172.17.0.1 (target) destination 172.17.0.2 (attacker)
python-requests/2.28.1

<img width="1112" alt="image" src="https://github.com/user-attachments/assets/93177cdc-2584-4816-8319-6ed32a97c221">

Attacker created a backdoor

<img width="742" alt="image" src="https://github.com/user-attachments/assets/a6c0af1a-2748-4ba4-b6c4-80a0d32d3c2a">
<img width="714" alt="image" src="https://github.com/user-attachments/assets/c872fb23-78e5-438e-86b7-0518be440872">

Tried to connect to 172.17.0.1 with ssh but I don't think it's a real IP. 
* 172.17.0.1 is a private IP address only used in internal network environs. 

Now what? 

*We need "key.pem" file to decrypt the TLS communication
*in terminal:
$ nano key.pem 

--> copied from -----Begin RSA Private Key----- to -----End RSA Private Key------

<img width="567" alt="image" src="https://github.com/user-attachments/assets/9dc62025-85cb-4ee3-a189-812c48ad262d">

*Wireshark: Preferences > Protocols > TLS > RSA keys list

<img width="771" alt="image" src="https://github.com/user-attachments/assets/f771edd9-4baf-4944-887e-cdca8011f540">

*Follow second HTTP stream to view plaintext

<img width="743" alt="image" src="https://github.com/user-attachments/assets/6ca55da5-8ae9-4d03-89ac-047c59d1b5d9">


