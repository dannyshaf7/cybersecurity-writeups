Tubes from US Cyber Games Summer 2024
Author: Unknown

<img width="498" alt="image" src="https://github.com/user-attachments/assets/02731ddb-baee-417f-a846-3e1de930addb">

Id_uscg contains private key, can connect through ssh
Gave the file the correct permissions using 

$ chmod 700 id_uscg

$ ssh -I id_uscg usc@tubes.challs.uscybergames.com

<img width="592" alt="image" src="https://github.com/user-attachments/assets/074c330c-ac12-4f79-aedd-2165d3ff1237">


*some tools are missing, searched to see what's available **tcdump!!

<img width="600" alt="image" src="https://github.com/user-attachments/assets/6e2a4a5c-b045-4b37-8a6d-d687f2c3680a">

Using tcpdump to watch traffic

$ tcpdump -I ens4 -A -c 5 (interface ens4, ascii output, capture 5 packets)

<img width="786" alt="image" src="https://github.com/user-attachments/assets/e6e81c7e-44c5-49af-b449-6e9d8341ff5b">

192.168.0.2.22 > 24.98.92.233.53586

Tried ssh, telnet, nmap, nc, appears to be down, all ports filtered or refused

192.168.0.2.22 > 75.68.2.51.63944

<img width="645" alt="image" src="https://github.com/user-attachments/assets/f5ac0326-cf12-4612-8443-69a98abb1b16">

*reviewing single connections on ports out of normal range

<img width="655" alt="image" src="https://github.com/user-attachments/assets/15dca5ae-0ab5-48ea-bc3c-6f6b50db6987">

*Packets are sending ascii art!!

<img width="662" alt="image" src="https://github.com/user-attachments/assets/455292ba-9a1d-4bd4-995b-9cb9a8f22f3c">

