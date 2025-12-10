# Setup Guide – Virtual Corporate Linux Network

## 1. Netzwerk
- Adapter 1: Host-Only
- Adapter 2: NAT

## 2. Statische IP (Netplan)
Server-IP:
192.168.56.10

## 3. Firewall
Aktivierung mit UFW
- SSH erlaubt
- SMB-Ports: 137, 138, 139, 445

## 4. Samba File Server
Freigaben:
- Public → freier Zugriff (Passwort erforderlich)
- Finance → geschützter Zugriff nur für finance

Benutzer:
- vboxuser
- finance

## 5. Windows Client Zugriff
Verbindung über:
\\192.168.56.10

Oder per Laufwerk:
P: → Public  
F: → Finance

## 6. Sicherheit
- SMB2 erzwungen
- Keine Guest-Anmeldung erlaubt
- Zugriff nur mit Authentifizierung

