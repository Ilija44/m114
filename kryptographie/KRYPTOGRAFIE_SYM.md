# Symmetrische Kryptographie 

## Aufgabe 2
DER ANGRIFF ERFOLGT ZUR TEEZEIT

DIE WUERFEL SIND GEFALLEN

ICH KAM SAH UND SIEGTE

TEILE UND HERRSCHE

## Aufgabe 3
Verschlüsselung des Wortes BEEF mit dem Schlüsselwort AFFE: BJJJ

Entschlüsselung des Geheimtexts WRKXQT mit dem Schlüsselwort SECRET: ENIGMA

Entschlüsselter Text der Vigenère-Chiffre: 
DER STAAT BIN ICH

ES IST AEUSSERST SCHWIERIG ZU REDEN OHNE VIEL ZU SAGEN

ICH MACHE MIT JEDER ERNENNUNG NEUNUNDNEUNZIG UNZUFRIEDENE UND EINEN UNDANKBAREN

LOUIS XIV

## Aufgabe 4
4711 ergibt binär 0001'0010'0110'0111

0001'0010'0110'0111 (Den Klartext...)

1000‘1101'1000‘1101 (...mit 2x wiederholtem Key XOR verknüpft...)

1001'1111'1110'1010 (...ergibt diese Chiffre)

### Aufgabe 5

1. **Virtuelle Maschine erstellen:**
   - Installiere VirtualBox und lade die Ubuntu-ISO herunter.
   - Erstelle eine neue VM in VirtualBox und installiere Ubuntu.
2. **SSH einrichten:**
   - Installiere `openssh-server` auf Ubuntu: `sudo apt-get install openssh-server`
   - Starte den SSH-Dienst: `sudo service ssh start`
3. **Verbindung überprüfen:**
   - Öffne auf deinem Windows-PC ein Terminal (CMD, PowerShell oder Git Bash).
   - Verbinde dich per SSH: `ssh username@ip-address`
4. **Graphische Anbindung:**
   - Möglich mit X11-Forwarding: `ssh -X username@ip-address`
   - Alternativ: Verwendung von Tools wie `VNC` oder `RDP`.

### Aufgabe 6


1. **HTTP-Verbindung (http://www.example.ch):**
   - Start Wireshark und wähle das Netzwerkinterface aus.
   - Filtern nach HTTP-Verkehr: `http`
   - Untersuchen der OSI-Schichten:
     - Layer 2 (Data Link): Ethernet-Frame
     - Layer 3 (Network): IP-Paket
     - Layer 4 (Transport): TCP-Segment
     - Layer 7 (Application): HTTP-Daten
2. **HTTPS-Verbindung (https://www.zkb.ch):**
   - Filtern nach HTTPS-Verkehr: `tls`
   - Untersuchen der OSI-Schichten:
     - Layer 2 (Data Link): Ethernet-Frame
     - Layer 3 (Network): IP-Paket
     - Layer 4 (Transport): TCP-Segment
     - Layer 7 (Application): TLS-Daten
   - Unterschiede: HTTPS ist verschlüsselt, HTTP nicht.
   - Zusatzfrage: Mit Wireshark kann man die besuchte Webseite anhand der Server-IP oder des SSL/TLS-Zertifikats ermitteln.

### Aufgabe 7

- **https://juergarnold.ch:**
  - Protokoll: HTTPS
  - Zertifikat: Über Let's Encrypt ausgestellt
- **https://www.zkb.ch:**
  - Protokoll: HTTPS
  - Zertifikat: Über eine größere Zertifizierungsstelle wie SwissSign ausgestellt

### Aufgabe 8
- **CAcert.org:** Bietet kostenlose digitale Zertifikate an, jedoch muss man sich durch einen Web-of-Trust-Mechanismus verifizieren lassen.
- **Let's Encrypt:** Bietet kostenlose, automatisierte und offene Zertifikate an. Es wird keine manuelle Verifizierung benötigt, sondern alles erfolgt automatisiert.

### Aufgabe 9

- **Domain Validated (DV):** Bestätigt nur die Domaininhaberschaft.
- **Organization Validated (OV):** Überprüft die Identität der Organisation.
- **Extended Validation (EV):** Führt eine erweiterte Überprüfung der Organisation durch und zeigt ein grünes Adressfeld im Browser.
- **Für einen Webshop:** EV-Zertifikat ist am besten geeignet, da es das höchste Vertrauen bietet.

### Aufgabe 10


- **OpenPGP:** Ein Standard zur Verschlüsselung und zum Signieren von Daten und E-Mails, der hauptsächlich auf Web of Trust basiert.
- **X.509:** Ein Standard für öffentliche Schlüsselzertifikate, der in hierarchischen PKI-Umgebungen verwendet wird und bei HTTPS verwendet wird.

### Aufgabe 11

1. **Client Hello:** Der Client sendet eine Anforderung an den Server mit unterstützten Verschlüsselungsmethoden.
2. **Server Hello:** Der Server antwortet mit der gewählten Verschlüsselungsmethode und dem Zertifikat.
3. **Zertifikatsüberprüfung:** Der Client überprüft das Serverzertifikat.
4. **Schlüsselgenerierung:** Der Client und der Server erzeugen gemeinsame Sitzungsschlüssel.
5. **Sichere Verbindung:** Die verschlüsselte Kommunikation beginnt.

### Aufgabe 12
- **S/MIME:** Secure/Multipurpose Internet Mail Extensions. Ein Standard zum Verschlüsseln und Signieren von E-Mails.

### Aufgabe 13
**Wie archiviert man verschlüsselten E-Mail-Verkehr aus gesetzlichen Gründen?**

- **Problem:** Verschlüsselte E-Mails können nicht einfach archiviert werden, da der Inhalt ohne den Schlüssel unzugänglich ist.

 ## PGP und OpenPGP

## Durchführung der Aufgaben mit Gpg4win/Kleopatra

### Aufgabe 1: GPG4WIN auf dem eigenen Notebook installieren
**Schritte:**
1. Besuche die Webseite [GPG4WIN herunterladen](https://www.gpg4win.de/).
2. Lade die Installationsdatei herunter und führe sie aus.
3. Folge den Installationsanweisungen, um GPG4WIN auf deinem System zu installieren.

### Aufgabe 2: Mit GPG4WIN/Kleopatra ein Schlüsselpaar erstellen
**a) Starten des gpg4win-Zertifikatsmanagers Kleopatra:**
- Öffne Kleopatra aus dem Startmenü.

**b) Erzeugen eines persönlichen Schlüsselpaars:**
- In Kleopatra auf `Datei` -> `Neues OpenPGP-Schlüsselpaar...` klicken.
- Name und eine Test-E-Mail-Adresse eingeben.
- Auf `Weiter` und dann auf `Erzeugen` klicken.
- Eine Passphrase erstellen und bestätigen.

**c) Passphrase:**
- Eine starke Passphrase erstellen und notieren.

**d) Exportieren des eigenen öffentlichen Schlüssels:**
- Den öffentlichen Schlüssel über `Datei` -> `Exportieren...` exportieren.
- Das exportierte ASC-File mit einem Texteditor überprüfen. Es sollte mit `BEGIN PGP PUBLIC KEY BLOCK` beginnen.
- Die Datei in `Ilija_Predolac_PublicKey.asc` umbenennen.

**e) Importieren von öffentlichen Schlüsseln:**
- Öffentliche Schlüssel von Kommunikationspartnern importieren, indem die `.asc`-Dateien in Kleopatra importiert werden.

**f) Testen des Schlüsseltauschs:**
- Öffentliche Schlüssel mit einem Partner austauschen und gegenseitig importieren.

### Aufgabe 20: Fremden Public-Key verifizieren
**Authentizität des Ausstellerschlüssels überprüfen:**
- Fingerprint des Schlüssels direkt mit dem Kommunikationspartner vergleichen.
- Schlüssel von einer vertrauenswürdigen Quelle beziehen oder durch persönliche Treffen verifizieren.

### Aufgabe 21: Frage zum OpenPGP-Schlüssel
**Erkennungsmerkmale von OpenPGP-Schlüsseln:**
- Besteht aus einem Public-Key und einem Private-Key.
- Beginnt mit `BEGIN PGP PUBLIC KEY BLOCK` im ASCII-Format.

### Aufgabe 22: X.509-Schlüsselpaar erstellen
**Erstellen des X.509-Schlüsselpaares:**
- In Kleopatra auf `Datei` -> `Neues Schlüsselpaar...` klicken.
- Option für X.509 auswählen und den Anweisungen folgen, um das Schlüsselpaar zu erstellen.
- Unterschiede: X.509 erfordert eine Zertifizierungsstelle (CA) zur Verifizierung und wird häufig für S/MIME verwendet, während OpenPGP ohne zentrale Autorität auskommt.

### Aufgabe 23: Mit Gpg4win/Kleopatra eine Nachricht verschlüsseln
**Nachricht verschlüsseln:**
- Eine beliebige Datei in Kleopatra auswählen und mit dem öffentlichen Schlüssel des Kommunikationspartners verschlüsseln.
- Die verschlüsselte Datei per E-Mail an Kollegen senden.
- Kollege sollte die Datei erfolgreich entschlüsseln können.

### Aufgabe 24: Mit Gpg4win/Kleopatra eine Nachricht signieren
**Nachricht signieren:**
- Eine beliebige Datei in Kleopatra auswählen und mit dem privaten Schlüssel signieren.
- Die signierte Datei per E-Mail an den Kommunikationspartner senden.
- Kommunikationspartner sollte die Signatur erfolgreich verifizieren können.

### Aufgabe 25: Mit Gpg4win/Kleopatra eine Nachricht verschlüsseln und signieren
**Nachricht verschlüsseln und signieren:**
- Eine beliebige Datei in Kleopatra auswählen, verschlüsseln und mit dem privaten Schlüssel signieren.
- Die verschlüsselte und signierte Datei per E-Mail an den Kommunikationspartner senden.
- Kommunikationspartner sollte die Datei erfolgreich entschlüsseln und die Signatur verifizieren können.


