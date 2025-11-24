# Bases du TCP/IP

## 1. Configuration réseau (ipconfig)

Commande :
ipconfig /all

Informations importantes :
- Adresse IPv4
- Masque de sous-réseau
- Passerelle
- Serveur DNS
- Adresse MAC
- DHCP activé ou non

---

## 2. Exemple d'analyse

Exemple typique sur une machine cliente :
```
IPv4 : 192.168.10.20
Masque : 255.255.255.0
Passerelle : 192.168.10.1
DNS : 192.168.10.10
DHCP activé : Oui
```

Interprétation :
- Le PC est sur le réseau interne 192.168.10.0/24
- La passerelle est correcte
- Le DNS pointe vers le serveur interne → OK

---

## 3. Commande Get-NetIPAddress (PowerShell)
Get-NetIPAddress | Where-Object {$_.AddressFamily -eq "IPv4"}

Informations :
- Adaptateur
- IP
- Préfixe
- InterfaceIndex


