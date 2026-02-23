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

### Kosteneffizienz
Beim Cloud Computing werden Computingdienste mit einem nutzungsbasierten Preismodell über das Internet bereitgestellt. In der Regel bezahlt man nur für die Clouddienste, die man auch wirklich verwendet.
Ein solches nutzungsbasiertes Modell bietet viele Vorteile, wie etwa:

- Keine Vorlaufkosten
- Kostspielige Infrastruktur, die Benutzer*innen möglicherweise nicht voll nutzen, muss nicht erworben und verwaltet werden.
- Bei höherem Bedarf können weitere Ressourcen dazugekauft werden.
- Die Möglichkeit, für weniger Ressourcen zu zahlen, wenn weniger benötigt werden

### Globale Reichweite: 
Microsoft betreibt Rechenzentren in über 60 Regionen weltweit. Das sorgt für geringe Latenzzeiten und Ausfallsicherheit.

### Sicherheit: 
Microsoft investiert Milliarden in die Cybersicherheit. Für Unternehmen ist es oft sicherer, Daten in der hochgesicherten Azure-Cloud zu speichern als auf einem schlecht gewarteten lokalen Server.

### Hybrid-Cloud: 
Ein großer Vorteil von Azure ist die nahtlose Verbindung mit lokaler Windows-Infrastruktur (Active Directory, Windows Server).

<img width="1610" height="908" alt="I0WL1cP7bJ" src="https://github.com/user-attachments/assets/91d63361-55ed-4c26-b525-93297f6f92cf" />

## Azure-Konten
Möchte man Azure Dienste erstellen und verwenden benötigt man ein Azure-Abonnement
Arbeitet man mit seinen eigenen Anwendungen und Geschäftsanforderungen, muss man ein Azure-Konto erstellen. Dabei wird ein Abonnement erstellt.
Sobald ein Azure-Konto erstellt wurde, können zusätzliche Abonnements erstellt werden. Beispielsweise kann ein Unternehmen ein einzelnes Azure-Konto für das Unternehmen und separate Abonnements für die Entwicklungs-, Marketing- und Vertriebsabteilungen verwenden. Sobald ein Azure-Abonnement erstellt wurde, kann mit dem Erstellen von Azure-Ressourcen innerhalb dieses Abonnements begonnen werden.

<img width="755" height="598" alt="brave_INF0lrltkG" src="https://github.com/user-attachments/assets/7a8d6f82-94c4-4203-9a07-1e068a366fc2" />


## Interaktion mit Azure
Mit Azure kann auf unterschiedliche Weise interagiert werden, wie z.B. über das Azure-Webportal oder über die Azure-Befehlszeilenschnittstelle (CLI) mit PowerShell- oder Bash-Befehlen.

### Zugreifen auf das Azure-Portal
Das Azure-Portal ist eine grafische Benutzeroberfläche (GUI) für die Interaktion mit Azure-Diensten. Hier kann man zu den verschiedenen Dienstbereichen navigieren, Abonnements und Konten verwalten, nach bestimmten Services und Einstellungen suchen etc..

Das Azure Portal erreicht man unter https://portal.azure.com 

<img width="1920" height="997" alt="brave_e5CjdDg0oA" src="https://github.com/user-attachments/assets/94f450b1-67e2-4c59-b172-75c84a83813b" />

Ist die Anmeldung beim Portal erfolgt, kann mithilfe der Schnitstelle zu Azure navigiert werden oder die Befehlszeilenschnittstelle (CLI) mit PowerShell- und BASH-Befehlen verwendet werden.

### Verwenden des Command Line Interface (CLI)

Um über das Azure-Portal auf CloudShell zuzugreifen, wählt man das CloudShell-Symbol aus:


<img width="1637" height="72" alt="brave_izNmGqEHFT" src="https://github.com/user-attachments/assets/5d1b8b06-3aa5-4cc3-8010-0e729d5da569" />

Indem man die Schaltfläche "Switch to ... (Zu ... wechseln)" auswählt, bzw. "PWSH" oder "BASH" eingibt, kann man schnell zwischen PowerShell und BASH in der CLI wechseln:

<img width="1055" height="292" alt="brave_LINAkUNvJX" src="https://github.com/user-attachments/assets/5cabc796-cab8-40a9-bb57-1683e3b41976" />

 Tipp:
Im PowerShell-Modus beginnt die Befehlszeile mit PS. Im BASH-Modus beginnt die Befehlszeile mit Dem Benutzer name@azure.

### Verwenden des interaktiven Azure CLI-Modus

Eine weitere Möglichkeit zur Interaktion ist die Verwendung des interaktiven Modus der Azure-CLI.
Dadurch wird das Verhalten der CLI so geändert, dass es einer integrierten Entwicklungsumgebung (IDE) ähnelt. Der interaktive Modus bietet Funktionen wie AutoVervollständigen, Befehlsbeschreibungen und sogar Beispiele. Der Interaktive Modus kann hilfreich sein, wenn man die Befehlszeile verwenden möchte, sich aber mit Bash und PowerShell nicht auskennt. 

Geben Sie ```az interactive``` ein, um in den interaktiven Modus zu wechseln.

Entscheiden Sie, ob Telemetriedaten gesendet werden sollen und geben entweder ```NO``` oder ```YES``` ein.

<img width="1078" height="652" alt="brave_Li5BgyB4wd" src="https://github.com/user-attachments/assets/9d27ae6d-7cd8-475d-99f9-53f131ec6da8" />

Nach der Initialisierung können Sie die Pfeiltasten oder die TAB-Taste verwenden, um Ihre Befehle zu vervollständigen. Der interaktive Modus ist speziell für Azure eingerichtet, sodass Sie az nicht eingeben müssen, um einen Befehl zu starten. Verwenden Sie den Befehl ```exit```, um den interaktiven Modus zu verlassen.



