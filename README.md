# Lernportfolio

Aufgabe 1:


<img width="805" alt="image" src="https://github.com/user-attachments/assets/471ae424-590d-4125-ae36-ca74c764fd03" />


Aufgabe 2:

# Kabelmaterial für die WG "La familia"

## Ausgewählte Materialien für Gigabit Ethernet (1000MBit/sec)

### 1. Ethernet-Litzenkabel (Patchkabel)

<img width="658" alt="image" src="https://github.com/user-attachments/assets/8471049e-c715-4fe4-95cc-45cb43031b8e" />

- **Material**: Cat6a S/FTP Patchkabel (Litze)
- **Kabeleigenschaften**: 
  - Frequenzbereich bis 500 MHz
  - 4x2xAWG26/7 (7-adrige Litze)
  - Doppelte Abschirmung (Geflecht + Folie)
  - LSZH-Mantel (halogenfrei)
  - Flexibel für bewegliche Anwendungen
- **Anbieter**: Reichelt Elektronik
- **Bestellnummer**: NETL CAT6A-10
- **Kosten**: 1,95€ pro Meter

### 2. Ethernet-Drahtkabel (Installationskabel)

![U-FTP-image-1024x652](https://github.com/user-attachments/assets/3c612386-ab5d-4f42-b334-ab27bb702c27)

- **Material**: Cat6a U/FTP Installationskabel (Volldraht)
- **Kabeleigenschaften**: 
  - Frequenzbereich bis 500 MHz
  - 4x2xAWG23/1 (Massivdraht)
  - Foliengeschirmte Einzelpaare
  - PE-Isolierung
  - Optimal für Festinstallation im Gebäude
- **Anbieter**: Conrad Electronic
- **Bestellnummer**: CONN-CAT6A-305
- **Kosten**: 0,85€ pro Meter (bei 305m Rolle)


Aufgabe 3:

<img width="571" alt="image" src="https://github.com/user-attachments/assets/8868a314-353e-478f-be29-2c21347d4014" />


Das oben sind die Musterlösungen unten ist meine Lösung.


```
Swisscom-Telefondose
         │
     [ADSL-Modem]
    ┌───┼────────┬────────┐
    │   │        │        │
Zimmer1 Zimmer2 Zimmer3
```

---


20.05.2025


Aufgabe 1:
⸻

Private IPv4-Adressbereiche

10   .0   .0.0   –   10   .255.255.255       Ehemals Class A-Adresse  
172.16 .0.0     –   172.31 .255.255         Ehemals Class B-Adresse  
192.168.0.0     –   192.168.255.255         Ehemals Class C-Adresse  


⸻

Spezialadressen

127.0.0.1                                  Localnet oder Loopbackadresse (Eigener Rechner)  
169.254.0.0 – 169.254.255.255              ZEROCONF/APIPA-Adressen bei DHCP-Ausfall  


⸻


Aufgabe 2:

⸻

✅ 10.11.12.4 /24

Netzmaske: 255.255.255.0

Netz-ID: 10.11.12

Host-ID: 4

Netzwerkadresse: 10.11.12.0

Broadcastadresse: 10.11.12.255

⸻

✅ 10.11.12.4 /16

Netzmaske: 255.255.0.0

Netz-ID: 10.11

Host-ID: 12.4

Netzwerkadresse: 10.11.0.0

Broadcastadresse: 10.11.255.255

⸻

✅ 10.11.12.4 /8

Netzmaske: 255.0.0.0

Netz-ID: 10

Host-ID: 11.12.4

Netzwerkadresse: 10.0.0.0

Broadcastadresse: 10.255.255.255

⸻



Aufgabe 3:


---

### 🔹 **10.0.0.0 /8**
- **Anzahl im Subnetz (Host-ID):** 2²⁴ = **16.777.216**
- **IP:** 10.0.0.0 bis 10.255.255.255  
- **PC (verwendbare Hosts):** **16.777.214** (abzüglich Netzwerk- und Broadcastadresse)

---

### 🔹 **10.0.0.0 /16**
- **Anzahl im Subnetz (Host-ID):** 2¹⁶ = **65.536**
- **IP:** 10.0.0.0 bis 10.0.255.255  
- **PC (verwendbare Hosts):** **65.534**

---

### 🔹 **10.0.0.0 /24**
- **Anzahl im Subnetz (Host-ID):** 2⁸ = **256**
- **IP:** 10.0.0.0 bis 10.0.0.255  
- **PC (verwendbare Hosts):** **254**

---



