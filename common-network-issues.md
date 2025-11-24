# Problèmes Réseau Courants & Solutions

## Problème 1 — Adresse IP APIPA (169.254.x.x)

Cause : DHCP indisponible  
Solution :  
- `ipconfig /renew`  
- Vérifier câble / Wi-Fi  
- Vérifier serveur DHCP

---

## Problème 2 — DNS non fonctionnel

Symptômes :
- Navigateur ne charge rien
- Outlook ne s’ouvre pas

Solutions :

ipconfig /flushdns

nslookup google.com

---

## Problème 3 — Ping OK mais sites indisponibles

→ Problème HTTPS ou certificat  
Tester :
Test-NetConnection google.com -Port 443

---

## Problème 4 — Connexion lente

Causes :
- saturation Wi-Fi
- interférences
- câble défectueux

---

## Problème 5 — Pas d’accès Internet

Tests :
- Ping 8.8.8.8
- ping passerelle
- check DNS
