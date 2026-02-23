# Microsoft-Azure-Grundlagen

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

Ist die Anmeldung beim Portal erfolgt, kann mithilfe der Schnitstelle zu Azure navigiert werden oder die Befehlszeilenschnittstelle (CLI) mit **PowerShell**- und **BASH**-Befehlen verwendet werden.

### Verwenden des Command Line Interface (CLI)

Um über das Azure-Portal auf CloudShell zuzugreifen, wählt man das CloudShell-Symbol aus:


<img width="1637" height="72" alt="brave_izNmGqEHFT" src="https://github.com/user-attachments/assets/5d1b8b06-3aa5-4cc3-8010-0e729d5da569" />

Indem man die Schaltfläche "Switch to ... (Zu ... wechseln)" auswählt, bzw. "PWSH" oder "BASH" eingibt, kann man schnell zwischen PowerShell und BASH in der CLI wechseln:

<img width="1055" height="292" alt="brave_LINAkUNvJX" src="https://github.com/user-attachments/assets/5cabc796-cab8-40a9-bb57-1683e3b41976" />

 Tipp:
Im PowerShell-Modus beginnt die Befehlszeile mit PS. Im BASH-Modus beginnt die Befehlszeile mit Dem Benutzer name@azure.

### Verwenden des interaktiven Azure CLI-Modus

Eine weitere Möglichkeit zur Interaktion ist die Verwendung des interaktiven Modus der Azure-CLI.
Dadurch wird das Verhalten der CLI so geändert, dass es einer integrierten Entwicklungsumgebung (IDE) ähnelt. Der interaktive Modus bietet Funktionen wie **AutoVervollständigen**, **Befehlsbeschreibungen** und sogar **Beispiele**. Der Interaktive Modus kann hilfreich sein, wenn man die Befehlszeile verwenden möchte, sich aber mit Bash und PowerShell nicht auskennt. 

Geben Sie ```az interactive``` ein, um in den interaktiven Modus zu wechseln.

Entscheiden Sie, ob Telemetriedaten gesendet werden sollen und geben entweder ```NO``` oder ```YES``` ein.

<img width="1078" height="652" alt="brave_Li5BgyB4wd" src="https://github.com/user-attachments/assets/9d27ae6d-7cd8-475d-99f9-53f131ec6da8" />

Nach der Initialisierung können Sie die Pfeiltasten oder die TAB-Taste verwenden, um Ihre Befehle zu vervollständigen. Der interaktive Modus ist speziell für Azure eingerichtet, sodass Sie az nicht eingeben müssen, um einen Befehl zu starten. Verwenden Sie den Befehl ```exit```, um den interaktiven Modus zu verlassen.


## Die physische Infrastruktur von Azure
Im Rahmen von Microsoft Azure fallen ständig Begriffe wie "Regionen", "Verfügbarkeitszonen", "Ressourcen", "Abbonements", etc. Wichtig ist es, zunächst die Kernkomponenten der Azure-Architektur zu verstehen. Diese können in zweit primäre Gruppen unterteilt werden:
Die **physische Infrastruktur** und die **Verwaltungsinfrastruktur**.

### Physische Infrastruktur

Die physische Infrastruktur von Azure beginnt mit Rechenzentren, also große Einrichtungen mit Hardware-Ressourcen, die in Racks angeordnet sind und über dedizierte Energie-, Kühl- und Netzwerkinfrastruktur verfügen. 

Azure verfügt weltweit über Rechenzentren, die in Azure-Regionen und Azure-Verfügbarkeitszonen gruppiert werden. 

#### Regionen

Mit "Region" ist ein geographischer Bereich auf der Erde gemeint, in dem sich mindestens ein, möglicherweise jedoch mehrere, nicht weit voneinander entfernt liegende Rechenzentren befinden, die über ein  Netzwerk mit geringer Latenz miteinander verbunden sind. 
Um Load-Balancing zu gewährleisten, weist Azure die Ressourcen innerhalb jeder Region auf intelligente Weise zu und kontrolliert sie. 

Stellt man eine Ressource in Azure bereit, muss man also oft die Region auswählen, in der die Ressource bereitgestellt werden soll. 

EIne Einsicht in die globale Infrastruktur und die verschiedenen Azure-Regionen findet man unter:
https://datacenters.microsoft.com/globe/

#### Verfügbarkeitszonen

Verfügbarkeitszonen sind physisch getrennte Rechenzentren in einer Azure-Region. Jede Verfügbarkeitszone besteht aus mindestens einem Rechenzentrum, dessen Stromversorgung, Kühlung und Netzwerkbetrieb unabhängig funktionieren. Sie sind als Isolationsgrenzen eingerichtet. Wenn eine Verfügbarkeitszone ausfällt, arbeitet die andere dennoch weiter. Verfügbarkeitszonen sind über sehr schnelle private Glasfasernetzwerke miteinander verbunden.

<img width="507" height="505" alt="brave_j6KHwhCtih" src="https://github.com/user-attachments/assets/a22ad2f1-9824-4199-9146-3f0f0faf5ae7" />

**Warum sind Verfügbarkeitszonen wichtig?**

Um sicherzustellen, dass Dienste und Daten einer Anwendung **redundant** sind, und Informationen geschützt sind, falls Fehler auftreten ist es wichtig, dass die zugrundeliegenden Hardwareumgebungen in **zweifacher Ausführung** eingerichtet sind. Hier kommen Verfügbarkeitszonen ins Spiel. 

Compute-, Speicher-, Netzwerk-, und Datenressourcen werden in einer Verfügbarkeitszone bereitgestellt und in andere Verfügbarkeitszonen **repliziert**. Somit wird für **Hochverfügbarkeit** der App gesorgt

Verfügbarkeitszonen sind in erster Linie für virtuelle Computer, verwaltete Datenträger, Lastenausgleiche und SQL-Datenbanken gedacht. Azure-Dienste, die Verfügbarkeitszonen unterstützen, können in drei Kategorien unterteilt werden:

**Zonale Dienste:** Sie weisen die Ressource fest einer bestimmten Zone zu (z. B. virtuelle Computer, verwaltete Datenträger oder IP-Adressen).

**Zonenredundante Dienste:** Die Plattform repliziert automatisch zonenübergreifend (z. B. zonenredundanter Speicher oder SQL-Datenbank).

**Nicht regionale Dienste:** Dienste sind immer in Azure-Geografien verfügbar und sowohl gegen zonenweite als auch regionsweite Ausfälle resilient.

Selbst mit der zusätzlichen Resilienz, die Verfügbarkeitszonen bieten, ist es möglich, dass ein Ereignis so groß sein könnte, dass es sich auf mehrere Verfügbarkeitszonen in einer einzelnen Region auswirkt. Um die Resilienz noch weiter zu steigern, bietet Azure Regionspaare.

#### Regionspaare

Die meisten Azure-Regionen werden mit einer anderen Region, die mindestens 480 km (300 Meilen) entfernt ist, innerhalb derselben Geografie (z. B. USA, Europa oder Asien) kombiniert. Dieser Ansatz ermöglicht die Replikation von Ressourcen innerhalb einer Geografie bei gleichzeitiger Verringerung der Wahrscheinlichkeit, dass Naturkatastrophen, Unruhen, Stromausfälle oder physische Netzwerkausfälle eine gesamte Region betreffen. Wenn eine Region in einem Paar beispielsweise von einer Naturkatastrophe betroffen ist, würden Dienste automatisch ein Failover in eine andere Region im zugehörigen Regionspaar ausführen.

Beispiele für Regionspaare in Azure sind „USA, Westen“ kombiniert mit „USA, Osten“ oder „Asien, Südosten“ kombiniert mit „Asien, Osten“. Da das Regionspaar direkt verbunden und dennoch weit genug voneinander entfernt ist, um im Fall regionaler Katastrophen nicht betroffen zu sein, können Sie damit zuverlässige Dienste und Datenredundanz gewährleisten.

<img width="1075" height="596" alt="brave_eymK5l90uv" src="https://github.com/user-attachments/assets/f7288940-ff6d-4388-9f5b-5ad2216762ea" />


## Die Verwaltungsinfrastruktur von Azure

Die Verwaltungsinfrastruktur umfasst Azure-Ressourcen sowie Ressourcengruppen, Abonnements und Konten. Das Verständnis der hierarchischen Struktur hilft dabei, Projekte und Produkte in Azure zu planen.

### Azure-Ressourcen und -Ressourcengruppen

Eine Ressource ist der grundlegende Baustein in Azure. Alles, was erstellt oder bereitgestellt wird, ist eine Ressource. Dazu gehören VMs, virtuelle Netzwerke, Datenbanken, Container, Virtueller Speicher, Cognitive Services usw...

Ressourcengruppen sind, wie der Name schon sagt, Gruppierungen von Ressourcen. Wird eine Ressource erstellt, muss diese in einer Ressourcengruppe platziert werden. 

Eine Ressourcengruppe kann viele Ressourcen enthalten, aber eine einzelne Ressource kann jeweils nur in einer Ressourcengruppe enthalten sein. Einige Ressourcen werden möglicherweise zwischen Ressourcengruppen verschoben.

Wird eine Ressource in eine neue Gruppe verschoben, ist sie anschließend nicht mehr der ehemaligen Gruppe zugeordnet. Außerdem ist ein schachteln der Ressourcengruppen nicht möglich, d.h Ressourcengruppe B kann nich in die Ressourcengruppe A eingeschlossen werden.

Wird eine Ressourcengruppe gelöscht, so werden alle in ihr enthaltenen Ressourcen gelöscht. 

Ressourcengruppen sollten nach der Struktur bereitgestellt werden, die den jeweiligen Anforderungen am besten entspricht, allgemeingültige Regeln zur verwendung von Ressourcengruppen gibt es nicht. 

## Azure-Abonnements

