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

Aufgabe 4:



---

### 🧮 **1. Paar**  
**PC1:** 192.168.1.23 / 255.255.255.0  
**PC2:** 192.168.1.176 / 255.255.255.0  

**Netzadresse beider:** 192.168.1.0  
✅ **Antwort:** **Ja**  
**Begründung:** Beide liegen im selben Subnetz (192.168.1.0/24)

---

### 🧮 **2. Paar**  
**PC1:** 192.168.3.23 / 255.255.0.0  
**PC2:** 192.168.246.29 / 255.255.0.0  

**Netzadresse beider:** 192.168.0.0  
✅ **Antwort:** **Ja**  
**Begründung:** Beide im selben Subnetz (192.168.0.0/16)

---

### 🧮 **3. Paar**  
**PC1:** 192.168.3.23 / 255.255.255.0 → Subnetz: 192.168.3.0  
**PC2:** 192.168.246.29 / 255.255.255.0 → Subnetz: 192.168.246.0  

❌ **Antwort:** **Nein**  
**Begründung:** Unterschiedliche Subnetze (192.168.3.0 ≠ 192.168.246.0)

---

### 🧮 **4. Paar**  
**PC1:** 10.34.233.27 / 255.0.0.0 → Subnetz: 10.0.0.0  
**PC2:** 10.167.246.178 / 255.0.0.0 → Subnetz: 10.0.0.0  

✅ **Antwort:** **Ja**  
**Begründung:** Beide im selben Subnetz (10.0.0.0/8)

---

### ✅ Zusammenfassung:

| Paar | Kommunizieren? | Begründung |
|------|----------------|------------|
| 1    | Ja             | Gleiche Netzadresse (/24) |
| 2    | Ja             | Gleiche Netzadresse (/16) |
| 3    | Nein           | Unterschiedliche Netzadressen (/24) |
| 4    | Ja             | Gleiche Netzadresse (/8) |






Aufgabe 5:



---

### 🧮 **1. Paar**
**PC1:** 10.34.233.27 / 255.0.0.0 → Subnetz: 10.0.0.0  
**PC2:** 10.34.233.27 / 255.255.255.0 → Subnetz: 10.34.233.0  

❌ **Antwort:** **Nein**  
**Begründung:** Unterschiedliche Subnetze → Kommunikation ohne Router nicht möglich

---

### 🧮 **2. Paar**
**PC1:** 10.34.258.21 / 255.255.255.0 → ungültige IP!  
→ 258 ist **kein gültiger Oktettwert** (max. 255)

❌ **Antwort:** **Nein**  
**Begründung:** IP-Adresse ungültig → Kommunikation nicht möglich

---

### 🧮 **3. Paar**
**PC1:** 172.16.1.55 / 255.0.0.0 → Subnetz: 172.0.0.0  
**PC2:** 172.33.5.27 / 255.0.0.0 → Subnetz: 172.0.0.0  

✅ **Antwort:** **Ja**  
**Begründung:** Beide im selben Netzbereich (Netzadresse 172.0.0.0/8)

---

### 🧮 **4. Paar**
**PC1:** 10.0.1.17 / 255.255.0.0 → Subnetz: 10.0.0.0  
**PC2:** 10.0.2.24 / 255.255.255.0 → Subnetz: 10.0.2.0  

❌ **Antwort:** **Nein**  
**Begründung:** Unterschiedliche Netzmasken → unterschiedliche Subnetze

---

### ✅ Zusammenfassung:

| Paar | Kommunizieren? | Begründung |
|------|----------------|------------|
| 1    | Nein           | Unterschiedliche Subnetze (/8 vs. /24) |
| 2    | Nein           | Ungültige IP-Adresse (258) |
| 3    | Ja             | Beide im selben Subnetz (/8) |
| 4    | Nein           | Unterschiedliche Netzbereiche (/16 vs. /24) |

Aufgabe 6:

<img width="773" alt="image" src="https://github.com/user-attachments/assets/a49b7e66-ceaf-4aba-87f3-44f6c840b4a7" />

17.05.2025



Aufgabe 1:
SAT Tabelle

bd
be
ae
aa, ab, ac, ad, bc, bb, bc



Aufgabe 2:
1. Was ist der Zweck der logischen Port-Nummer?
Sie identifiziert eindeutig eine Anwendung oder einen Dienst auf einem Host und ordnet eingehende Datenpakete der richtigen Anwendung zu.

2. Wie viele Bit hat die Portnummer und was ist ihr Wertebereich?
16 Bit, Wertebereich: 0-65535

3. Was ist der Wertebereich der System Ports (Wellknown Ports)?
0-1023

4. Was ist der Wertebereich der Registered Ports (User Ports)?
1024-49151

5. Was ist der Wertebereich der Dynamic Ports?
49152-65535

6. Über welchen Portbereich kann das Betriebssystem frei verfügen?
49152-65535 (Dynamic Ports)

7. Protokollabkürzungen und System-Portnummern:
- HTTP: Hypertext Transfer Protocol (Port 80)
- HTTPS: Hypertext Transfer Protocol Secure (Port 443)
- FTP: File Transfer Protocol (Port 21)
- SMTP: Simple Mail Transfer Protocol (Port 25)
- POP3: Post Office Protocol Version 3 (Port 110)
- POP3S: Post Office Protocol Version 3 Secure (Port 995)
- IMAP: Internet Message Access Protocol (Port 143)
- IMAPS: Internet Message Access Protocol Secure (Port 993)
- Echo/Ping: Echo Protocol (Port 7)
- DNS: Domain Name System (Port 53)





### 1. **Absoluter und relativer Pfad**
- **Absoluter Pfad**: Gibt den vollständigen Weg zu einer Datei oder einem Verzeichnis an – vom **Stammverzeichnis (Root)** bis zum Ziel.  
  Beispiel (Windows): `C:\Benutzer\Max\Dokumente\Datei.txt`  
  Beispiel (Linux): `/home/max/dokumente/datei.txt`

- **Relativer Pfad**: Gibt den Weg **relativ zum aktuellen Verzeichnis** an.  
  Beispiel: `..\Bilder\foto.jpg` (ein Verzeichnis hoch, dann in „Bilder“ gehen)

---

### 2. **Pfadangaben: Bedeutung von `.` und `..`**
- `.` (Punkt): Steht für das **aktuelle Verzeichnis**  
- `..` (zwei Punkte): Steht für das **übergeordnete Verzeichnis**

Beispiel:  
Angenommen, du bist in `C:\Benutzer\Max\Dokumente`  
- `.` → bleibt in `Dokumente`  
- `..` → geht zurück zu `Max`  
- `..\Bilder` → geht zu `C:\Benutzer\Max\Bilder`

---

### 3. **FAT und NTFS – Bedeutung und Unterschiede**
- **FAT** (File Allocation Table):  
  Ein älteres Dateisystem (z. B. FAT32), weit verbreitet bei USB-Sticks und Speicherkarten.  
  - Vorteile: Kompatibel mit fast allen Betriebssystemen  
  - Nachteile: Begrenzte Dateigröße (max. 4 GB), keine Benutzerrechte, weniger sicher

- **NTFS** (New Technology File System):  
  Modernes Windows-Dateisystem  
  - Vorteile: Unterstützt große Dateien, Rechteverwaltung, Verschlüsselung, Journaling (Datensicherheit)  
  - Nachteile: Nicht vollständig kompatibel mit älteren Systemen oder macOS ohne Zusatzsoftware



---

### **1. Wieso Benutzer-Accounting?**

**Benutzer-Accounting** bedeutet, dass Aktivitäten von Benutzern im System **protokolliert und überwacht** werden.

**Ziele und Gründe:**
- **Sicherheit**: Nachvollziehbarkeit, wer was gemacht hat
- **Missbrauch erkennen**: Unberechtigte Zugriffe entdecken
- **Abrechnung**: Nutzung von Ressourcen (z. B. Druck, Speicher, Serverzeit) erfassen
- **Verantwortung zuweisen**: Jede Aktion ist einem Benutzer zugeordnet
- **Audits & Compliance**: Vorschriften und Richtlinien einhalten

---

### **2. Was will man erreichen, wenn man Zugriffsrechte gruppenweise erteilt?**

**Gruppenbasierte Rechtevergabe bedeutet:**
- Benutzer werden in **Gruppen** (z. B. „Buchhaltung“, „IT“) eingeteilt
- Zugriffsrechte werden **einmal pro Gruppe** vergeben, nicht pro Person

**Vorteile/Ziele:**
- **Effizienz**: Rechteverwaltung ist einfacher und schneller
- **Übersichtlichkeit**: Klare Struktur, wer worauf zugreifen darf
- **Wartbarkeit**: Neue Benutzer müssen nur der richtigen Gruppe zugeordnet werden
- **Fehlervermeidung**: Geringeres Risiko falscher Rechtevergabe

---

### **3. Wann lokale, wann zentrale Benutzerverwaltung sinnvoll?**

| **Lokale Benutzerverwaltung** | **Zentrale Benutzerverwaltung** |
|-------------------------------|---------------------------------|
| Benutzerkonten sind **nur auf einem Gerät** gespeichert | Benutzerkonten sind **netzwerkweit zentral verwaltet** (z. B. per Active Directory) |
| **Sinnvoll bei:** Einzelplatzrechnern, kleinen Netzwerken, ohne Server | **Sinnvoll bei:** Firmen, Schulen, großen Netzwerken |
| Geringer Verwaltungsaufwand | Einheitliche Verwaltung vieler Benutzer |
| Keine Abhängigkeit vom Netzwerk | Benutzer können sich **an jedem Gerät im Netzwerk anmelden** |

**Kurz:**
- **Lokal**, wenn du **wenige Geräte oder Benutzer** hast.
- **Zentral**, wenn du **viele Benutzer oder Geräte im Netzwerk** verwalten willst.

---


**1. Vererbung von Zugriffsrechten:**
Unter Vererbung von Zugriffsrechten versteht man das automatische Übertragen von Berechtigungen von übergeordneten Ordnern auf untergeordnete Dateien und Ordner. Wenn einem Benutzer Zugriffsrechte auf einen Hauptordner gewährt werden, erben alle darin enthaltenen Unterordner und Dateien standardmäßig diese Berechtigungen, es sei denn, sie werden explizit überschrieben.

**2. Kommando \\10.0.1.100\projekte2024:**
Dies ist ein UNC-Pfad (Universal Naming Convention), der auf einen Netzwerkpfad verweist. Er bedeutet:
- 10.0.1.100 = IP-Adresse eines Servers im Netzwerk
- projekte2024 = Name der freigegebenen Ressource/des freigegebenen Ordners
Der Pfad stellt eine Verbindung zu einem geteilten Ordner auf einem Netzwerkcomputer her.

**3. USB-Stick mit sensiblen Daten verloren:**
**Ja, Sie sollten sich definitiv Sorgen machen!** Bei FAT32 sind Daten nicht verschlüsselt und leicht zugänglich. Sofortmaßnahmen:
- Alle gespeicherten Passwörter sofort ändern
- Cloud-Zugänge überprüfen und Sitzungen beenden
- Kreditkarten sperren lassen oder Banken kontaktieren
- Falls möglich, Remote-Löschung aktivieren

**4. NTFS USB-Stick Sicherheit:**
Beim korrekten Auswerfen werden die Daten **nicht automatisch gelöscht** - sie bleiben auf dem Stick. Der Zugriff wird nur **verweigert**, wenn:
- NTFS-Berechtigungen korrekt gesetzt sind
- Der Stick mit Verschlüsselung (BitLocker) geschützt ist
- Passwortschutz aktiviert wurde

**Empfehlung:** Für sensible Daten immer Verschlüsselung verwenden, nicht nur auf NTFS-Berechtigungen vertrauen.


Hier das Subnetting für 10.0.0.0/16 mit neun /24-Subnetzen A–I und die PC-Konfigurationen.

Aufgabe Logische Topologie der Firma Muster GmbH

1. Übersicht Subnetze A–I (/24)

Subnetz	Netzadresse	Broadcast	Maske

A	10.0.0.0	10.0.0.255	255.255.255.0 (/24)

B	10.0.1.0	10.0.1.255	255.255.255.0 (/24)

C	10.0.2.0	10.0.2.255	255.255.255.0 (/24)

D	10.0.3.0	10.0.3.255	255.255.255.0 (/24)

E	10.0.4.0	10.0.4.255	255.255.255.0 (/24)

F	10.0.5.0	10.0.5.255	255.255.255.0 (/24)

G	10.0.6.0	10.0.6.255	255.255.255.0 (/24)

H	10.0.7.0	10.0.7.255	255.255.255.0 (/24)

I	10.0.8.0	10.0.8.255	255.255.255.0 (/24)




2. PC-Konfiguration (IP, Maske, Gateway)

Subnetzmaske für alle PCs: 255.255.255.0 (/24)

Gateway pro Subnetz: 10.0.X.1 (X = Subnetz-Index A=0, B=1, …, I=8)

PC	Subnetz	IP-Adresse	Maske	Standard-Gateway

A-PC1	A	10.0.0.2	255.255.255.0	10.0.0.1

A-PC2	A	10.0.0.3	255.255.255.0	10.0.0.1

B-PC1	B	10.0.1.2	255.255.255.0	10.0.1.1

B-PC2	B	10.0.1.3	255.255.255.0	10.0.1.1

C-PC1	C	10.0.2.2	255.255.255.0	10.0.2.1

C-PC2	C	10.0.2.3	255.255.255.0	10.0.2.1

D-PC1	D	10.0.3.2	255.255.255.0	10.0.3.1

D-PC2	D	10.0.3.3	255.255.255.0	10.0.3.1

E-PC	E	10.0.4.2	255.255.255.0	10.0.4.1


## 01.07.2025


---

### **1. Displayfilter für das Anpingen eines Rechners**
**Antwort:**  
`icmp`

---

### **2. Kommando, um den Lokalhost anzupingen**
**Antwort:**  
```bash
ping 127.0.0.1
```

---

### **3. Ping an den Lokalhost – Was zeigt Wireshark?**
**Antwort:**  
Wireshark zeigt ICMP-Pakete (Echo Request und Echo Reply), allerdings nur, wenn der Netzwerkverkehr über eine Netzwerkschnittstelle läuft. Beim `127.0.0.1`-Ping (Loopback) wird meist **kein Paket** in Wireshark sichtbar, da es die Netzwerkschnittstelle nicht verlässt. Nur mit spezieller Loopback-Erfassung sichtbar.

---

### **4. Wie findet man die Router-IP des lokalen Netzwerks?**
**Antwort:**  
Über die Kommandozeile:
```bash
ipconfig (Windows)
ip route | grep default (Linux/Mac)
```
Dort steht die **Default Gateway IP-Adresse**, also die Router-IP.

---

### **5. Router anpingen – Wireshark-Analyse**
**Antwort:**  
Es werden ICMP Echo Requests an den Router gesendet und Echo Replies empfangen. Wireshark zeigt:
- ICMP Pakete
- Ziel-IP ist die des Routers
- MAC-Adresse des Routers als Empfänger (Layer 2)

---

### **6. Gibt es bei Ping einen OSI-Layer 4 (Transport-Layer)?**
**Antwort:**  
**Nein.** ICMP gehört direkt zum **Netzwerk-Layer (Layer 3)** und nutzt keinen Transport-Layer wie TCP oder UDP.

---

### **7. DNS-Server herausfinden**
**Antwort:**  
- Windows: `ipconfig /all` → Eintrag "DNS-Server"
- Linux/Mac: `cat /etc/resolv.conf`  
Hier steht die IP-Adresse des verwendeten DNS-Servers.

---

### **8. DNS-Abfrage aufzeichnen und analysieren**
**Antworten:**
- **Displayfilter für DNS:**  
  `dns`
- **DNS-Protokoll:**  
  **UDP** (Standard), TCP nur bei großen Antworten oder Zonenübertragungen
- **Portnummer:**  
  UDP **Port 53**

---

### **9. HTTP-GET analysieren (http://www.example.ch)**
- **Displayfilter:**  
  `http && ip.addr == [Webserver-IP]`
- **Layer-Analyse:**
  - a. **MAC-Adressen (OSI Layer 2):**  
    Absender: MAC-Adresse des PCs  
    Empfänger: MAC-Adresse des Routers oder Webservers (je nach Netzwerk)
  - b. **IP-Adressen (OSI Layer 3):**  
    Absender: IP des PCs  
    Empfänger: IP des Webservers (`www.example.ch`)
  - c. **Ports (OSI Layer 4):**  
    Absender-Port: Zufälliger hoher TCP-Port (z.B. 49123)  
    Empfänger-Port: TCP **Port 80** (HTTP)
  - d. **Anwendungsschicht (OSI Layer 7):**  
    HTTP GET-Request sichtbar. Danach folgt HTML-Datenübertragung – sichtbar als Text (HTML, CSS etc.)

---

### **10. HTTPS mit www.zkb.ch analysieren**

- **a. TLS – OSI-Schicht:**  
  **Layer 6** (Präsentationsschicht). TLS verschlüsselt Anwendungen wie HTTP.

- **Displayfilter für TLS:**  
  `ssl.handshake.extensions_server_name`

- **b. IP-Adresse von www.zkb.ch:**  
  Durch DNS-Request oder `nslookup www.zkb.ch`

- **c. MAC-Adressen (Layer 2):**  
  Absender: MAC-Adresse des PCs  
  Empfänger: MAC-Adresse des Routers (nicht direkt die des Webservers, da über Internet)

- **d. IP-Adressen (Layer 3):**  
  Absender: Lokale IP-Adresse  
  Empfänger: IP-Adresse des Webservers (ZKB)

- **e. Ports (Layer 4):**  
  Absender-Port: Zufälliger TCP-Port  
  Empfänger-Port: TCP **Port 443** (HTTPS)

- **f. Application-Layer:**  
  Inhalte sind verschlüsselt (nicht sichtbar wie bei HTTP).  
  Sichtbar bleibt:
  - **SNI (Server Name Indication)** beim TLS-Handshake
  - **Ziel-Webseite (Hostname)**  
  - **Handshake-Informationen**
  - **Zertifikate**

---

### **11. Eigene Dienst-Analyse (Beispiel: DHCP)**

- **Gewählter Dienst:** DHCP (Dynamic Host Configuration Protocol)
- **Well-Known-Portnummern:**  
  - Server: UDP **Port 67**  
  - Client: UDP **Port 68**
- **Verwendeter Displayfilter:**  
  `bootp` (für DHCP)
- **Vorgehen:**
  - Netzwerkschnittstelle auswählen
  - Wireshark-Aufzeichnung starten
  - DHCP-Anfrage auslösen (z.B. durch `ipconfig /release` + `ipconfig /renew` unter Windows)
  - Pakete analysieren: DHCP Discover, Offer, Request, ACK


