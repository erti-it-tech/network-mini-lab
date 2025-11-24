# Tests DNS

La résolution DNS est essentielle pour la connectivité réseau et Outlook/M365.

---

## 1. Test simple
nslookup google.com

Vérifie :
- si le DNS répond
- l’adresse du serveur DNS utilisé

---

## 2. Résolution DNS interne

Dans un domaine AD :
nslookup server.lab.local

---

## 3. Test via Test-NetConnection
Test-NetConnection -ComputerName outlook.office365.com -Port 443

Affiche :
- DNS OK ?
- Port 443 ouvert ?
- Latence ?

---

## 4. Problèmes DNS typiques

- DNS défini sur 8.8.8.8 → pas bon en entreprise AD  
- DNS corrompu dans Windows  
- DNS ne pointe pas vers le serveur interne  
- Cache DNS saturé → solution :
ipconfig /flushdns



