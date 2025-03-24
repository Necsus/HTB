#NMAP SCAN

TCP
nmap -sV -sC -Pn -oA {name} {host}

UDP
nmap -sU --top-ports 100 -Pn -oA {name} {host}

SYNC TIME FOR KERBEROS SYSTEM
timedatectl set-ntp off &
sudo ntpdate <host>
