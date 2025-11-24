# Tests Ping & Tracert

## 1. Test de connectivité général
ping 8.8.8.8

Si OK → interface réseau fonctionnelle  
Si pas OK → problème IP / route / driver

---

## 2. Test DNS via ping
ping google.com

Si 8.8.8.8 répond mais pas google.com → problème DNS.

---

## 3. Tracert
tracert outlook.office365.com

Permet de voir :
- les routeurs traversés
- où le trafic est bloqué

---

## 4. Test port 443
Test-NetConnection -ComputerName google.com -Port 443

Résultat utile pour :
- Outlook
- Teams
- Sites HTTPS





