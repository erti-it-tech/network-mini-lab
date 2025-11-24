# Tests DHCP

## 1. Vérifier si l'adresse est obtenue via DHCP
ipconfig /all | findstr "DHCP"

---

## 2. Libèrer l'adresse IP
ipconfig /release

---

## 3. Renouveller l’adresse IP
ipconfig /renew

---

## 4. Problèmes DHCP typiques

- Adresse en 169.254.x.x → **pas de DHCP**
- Serveur DHCP hors ligne
- PC trop loin dans le réseau / VLAN
- Borne Wi-Fi en panne
- Câble non connecté

---

## 5. Vérification passerelle
ping 192.168.10.1

Si la passerelle répond → le réseau local est OK.

