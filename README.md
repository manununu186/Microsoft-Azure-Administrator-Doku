# Microsoft-Azure-Administrator-Doku

## Was ist MS Azure?

Microsoft Azure ist eine umfassende Cloud-Computing-Plattform von Microsoft.
Ansttatt eigene Server On-Premise oder Rechenzentren werden Rechenleistung, 
Speicherplatz und Software-Dienste über das Internet gemietet.

Azure bietet über 200 Produkte und Dienstleistungen an, die sich grob in drei Kategorien unterteilen lassen:

### IaaS (Infrastructure as a Service):
Das ist die unterste Ebene. Man mietet virtuelle Hardware (Server, Netzwerke, Speicher) und ist selbst für das Betriebssystem und die Absicherung verantwortlich.

### PaaS (Platform as a Service):
Hier stellt Azure die Umgebung bereit, damit Entwickler Apps bauen können, ohne sich um die darunterliegende Server-Infrastruktur kümmern zu müssen (z. B. Azure SQL-Datenbanken).

### SaaS (Software as a Service):
Fertige Anwendungen, die über die Cloud laufen. (Wobei Microsoft hier meist auf Microsoft 365 verweist, das eng mit Azure verzahnt ist).


## Modell der gemeinsamen Verantwortung
Mit dem Modell der gemeinsamen Verantwortung werden die Verantwortlichkeiten über die jeweiligen Komponenten eines Systems zwischen dem Cloudanbieter und dem Verbraucher geteilt.
Je nach Clouddiensttyp liegen die Verantwortlichkeiten über Daten, Hardware, Netzwerk, Infrastruktur, Rechenzentrum etc. beim Cloudanbieter, beim Verbraucher oder wird geteilt:

<img width="1077" height="637" alt="brave_Y1wd1zCtuV" src="https://github.com/user-attachments/assets/344f71e6-9e45-4c6f-b64f-f37422df8349" />

Wer einen Cloudanbieter verwenden, ist immer für Folgendes verantwortlich:

- Die in der Cloud gespeicherten Informationen und Daten
- Geräte, die eine Verbindung mit Ihrer Cloud herstellen dürfen (Mobiltelefone, Computer usw.)
- Die Konten und Identitäten der Personen, Dienste und Geräte innerhalb Ihrer Organisation
 
Der Cloudanbieter ist immer für Folgendes verantwortlich:
- Das physische Rechenzentrum
- Das physische Netzwerk
- Die physischen Hosts
  
Das Dienstmodell bestimmt die Verantwortung für Dinge wie:
- Betriebssysteme
- Netzwerksteuerung
- Anwendungen
- Identität und Infrastruktur

## Warum nutzt man Azure?
### Skalierbarkeit: 
Wenn eine Website des Kunden plötzlich Millionen von Aufrufen hat, schaltet Azure automatisch mehr Leistung dazu. Wenn der Ansturm vorbei ist, regelt es wieder herunter.

### Globale Reichweite: 
Microsoft betreibt Rechenzentren in über 60 Regionen weltweit. Das sorgt für geringe Latenzzeiten und Ausfallsicherheit.

### Sicherheit: 
Microsoft investiert Milliarden in die Cybersicherheit. Für Unternehmen ist es oft sicherer, Daten in der hochgesicherten Azure-Cloud zu speichern als auf einem schlecht gewarteten lokalen Server.

### Hybrid-Cloud: 
Ein großer Vorteil von Azure ist die nahtlose Verbindung mit lokaler Windows-Infrastruktur (Active Directory, Windows Server).
