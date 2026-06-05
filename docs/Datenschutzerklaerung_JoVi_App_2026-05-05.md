# DatenschutzerklÃ¤rung fÃ¼r die JoVi-App

Rechtsversion: 2026-05-11.de-en.v1
GeprÃ¼ft fÃ¼r App-Version: 2.1.5+261560764

Stand: 05.05.2026

## 1. Verantwortlicher

Verantwortlich fÃ¼r die Verarbeitung personenbezogener Daten im Sinne der Datenschutz-Grundverordnung ist:

Johannes Vilsmeier  
BlÃ¼tenstr. 11  
71384 Weinstadt  
E-Mail: developer.joviapp@gmail.com  
Datenschutz-Kontakt: developer.joviapp@gmail.com

## 2. Gegenstand der App

Die JoVi-App ist eine App fÃ¼r Bestell-, Team- und StatistikablÃ¤ufe im Gastronomie-, Veranstaltungs- oder Vereinsumfeld. Nach dem geprÃ¼ften Projektstand gibt es insbesondere zwei Nutzungsarten:

- lokalen Solo-Betrieb mit Speicherung auf dem EndgerÃ¤t
- cloudgestÃ¼tzten Team-Betrieb mit Anmeldung, Teamverwaltung, gemeinsamen Bestellungen, AktivitÃ¤tsprotokollen, Statistiken und optionalen Pro-Abonnements

## 3. Verarbeitete Daten

### 3.1 Lokal gespeicherte Daten

Im lokalen Betrieb speichert die App Daten insbesondere mit lokalem App-Speicher, Hive und SharedPreferences. Dazu kÃ¶nnen insbesondere gehÃ¶ren:

- MenÃ¼s und MenÃ¼positionen
- Tischbestellungen
- Kassier- und Zahlungsdaten
- Tischlayout und Tischnamen
- App-Einstellungen, Sprache, UI-Skalierung und sonstige BedienprÃ¤ferenzen
- lokale Markierungen, Lese- und Ausblendstatus innerhalb der App
- lokale Verlaufsinformationen zu verlassenen Teams

Diese Daten bleiben grundsÃ¤tzlich auf Ihrem EndgerÃ¤t, soweit Sie keine Cloud-, Export- oder Teilen-Funktionen nutzen.

### 3.2 Konto- und Anmeldedaten

Bei Nutzung von Cloud- oder Pro-Funktionen verarbeitet die App Authentifizierungs- und Profildaten Ã¼ber Firebase Authentication. Je nach gewÃ¤hlter Anmeldeart kÃ¶nnen insbesondere verarbeitet werden:

- Benutzer-ID (UID)
- Anzeigename
- E-Mail-Adresse
- Profilbild-URL
- Information, ob ein Konto anonym genutzt wird

Der aktuelle Code sieht Anmeldungen Ã¼ber Google, Apple und eine anonyme Anmeldung fÃ¼r bestimmte Szenarien vor.

### 3.3 Team- und Kollaborationsdaten

Im Team-Modus werden Daten in Firebase Firestore verarbeitet. Dazu gehÃ¶ren je nach Nutzung insbesondere:

- Teamname
- Admin-ID
- Einladungs- oder Join-Code
- Teamstatus, Erstellungs- und SchlieÃŸungszeitpunkte
- Mitgliederdaten wie Anzeigename, Initialen, Rolle, Mitgliedsstatus und Zeitpunkte von Beitritt oder Austritt
- Join-Requests mit Anzeigename und Antragszeitpunkt
- gemeinsame MenÃ¼s
- Tischbestellungen
- ZahlungsdatensÃ¤tze
- Tischkonfigurationen
- AktivitÃ¤ts- und Systemprotokolle mit Text, Zeitstempel, Sendername, Sender-ID und Metadaten
- abgeleitete Tages-Snapshots fÃ¼r Statistikzwecke
- MitgliedschaftseintrÃ¤ge unter dem jeweiligen Benutzerkonto

Wenn Nutzer in Freitextfeldern oder Teambezeichnungen personenbezogene Angaben eintragen, kann die App auch solche Inhalte verarbeiten.

### 3.4 Abonnement- und Kaufdaten

Bei Nutzung kostenpflichtiger Pro-Funktionen verarbeitet die App abonnementsbezogene Daten. Dazu gehÃ¶ren dem geprÃ¼ften Code nach insbesondere:

- Produkt-ID des Abonnements
- Plattform des Kaufs
- Kauf-ID oder transaktionsbezogene Kennung
- serverseitige Verifizierungsdaten des jeweiligen Store-Kaufs
- Validierungsstatus und Validierungszeitpunkt
- Ablaufdatum des Abonnements
- Zuordnung eines Kauf-Tokens zu einer Benutzer-ID
- Pro-Status des Benutzerkontos

Die eigentliche Zahlungsabwicklung erfolgt Ã¼ber den jeweiligen App-Store. VollstÃ¤ndige Zahlungsdaten wie Kreditkarten- oder Bankdaten werden nach dem erkennbaren Projektstand nicht von der App selbst gespeichert.

UnabhÃ¤ngig davon verarbeitet die App eigene abonnementsbezogene Nachweis-, PrÃ¼f- und Statusdaten, soweit dies fÃ¼r die technische Validierung eines Kaufs, die Missbrauchsabwehr, die Zuordnung eines Kaufs zu einem Benutzerkonto und die Freischaltung oder EinschrÃ¤nkung von Pro-Funktionen erforderlich ist. Dazu kÃ¶nnen insbesondere in Firestore eingereichte Kaufnachweise, serverseitige PrÃ¼fergebnisse, Token-Zuordnungen und Statusfelder zum Pro-Abonnement gehÃ¶ren.

Nach dem aktuellen technischen Stand werden diese Datenarten mit unterschiedlichen LÃ¶schfristen behandelt. Kurzlebige technische Fehler- und PrÃ¼fdatensÃ¤tze zu eingereichten Kaufnachweisen werden kÃ¼rzer aufbewahrt als erfolgreich validierte Kaufnachweise. Reine Token-Zuordnungen zur technischen Zuordnung spÃ¤terer Store-Ereignisse kÃ¶nnen lÃ¤nger gespeichert werden als die eigentlichen Receipt-DatensÃ¤tze.

### 3.5 Export-, Import- und Freigabedaten

Die App bietet Export-, Import-, Download-, Ã–ffnen- und Teilen-Funktionen. Dabei kÃ¶nnen insbesondere verarbeitet oder an von Ihnen ausgewÃ¤hlte Ziele Ã¼bergeben werden:

- MenÃ¼dateien im .jovi-Format
- CSV-, HTML- und PDF-Exporte
- Statistikdateien
- Inhalte aus lokalen oder cloudbasierten DatenbestÃ¤nden

Wenn Sie eine Teilen-, Ã–ffnen- oder Speichern-Funktion verwenden, werden Daten an die von Ihnen ausgewÃ¤hlte Ziel-App, Dateiablage oder Systemfunktion Ã¼bergeben. Ab diesem Zeitpunkt gelten zusÃ¤tzlich deren Datenschutzbedingungen.

### 3.6 Kamera- und Scan-Funktionen

Der aktuelle Code verwendet eine Scanner-Funktion fÃ¼r QR- oder kameragestÃ¼tzte VorgÃ¤nge. Die Kamera wird nur genutzt, wenn Sie die entsprechende Funktion aktiv aufrufen.

### 3.7 Technische und betriebliche Daten

Zur Bereitstellung der App kÃ¶nnen auÃŸerdem technische Metadaten verarbeitet werden, insbesondere:

- Plattform und Betriebssystemkontext
- App-Version und Build-Nummer
- Zeitstempel von VorgÃ¤ngen
- Fehler- und Statusinformationen innerhalb der App- und Cloud-AblÃ¤ufe
- Berechtigungs- und Sicherheitsstatus bei Zugriffen auf Cloud-Daten

Aus dem geprÃ¼ften Code ergibt sich kein eigenstÃ¤ndiger Einsatz von Werbetracking, Werbe-SDKs oder klassischem Nutzerprofiling.

## 4. Zwecke der Verarbeitung

Wir verarbeiten Daten insbesondere zu folgenden Zwecken:

- Bereitstellung der App-Funktionen
- Speicherung und Synchronisierung von Bestellungen, MenÃ¼s, Teamdaten und Statistiken
- Benutzeranmeldung und Kontoverwaltung
- Teamverwaltung und Nachvollziehbarkeit von Team-AktivitÃ¤ten
- PrÃ¼fung und Durchsetzung von Berechtigungen und Sicherheitsregeln
- Abwicklung und Validierung von Pro-Abonnements
- Export, Import, Ã–ffnen und Teilen von Inhalten auf Wunsch der Nutzer
- Fehleranalyse, Missbrauchsvermeidung und technische StabilitÃ¤t

## 5. Rechtsgrundlagen

Soweit die DSGVO anwendbar ist, stÃ¼tzen wir die Verarbeitung insbesondere auf folgende Rechtsgrundlagen:

- Art. 6 Abs. 1 lit. b DSGVO fÃ¼r die Bereitstellung vertraglich oder vorvertraglich angefragter App-Funktionen
- Art. 6 Abs. 1 lit. f DSGVO fÃ¼r Sicherheits-, Missbrauchsabwehr-, StabilitÃ¤ts- und Verwaltungszwecke
- Art. 6 Abs. 1 lit. a DSGVO, soweit Sie freiwillig Funktionen wie externe Freigaben, Kameraeinsatz oder bestimmte Login-Verfahren nutzen
- Art. 6 Abs. 1 lit. c DSGVO, soweit rechtliche Aufbewahrungs- oder Nachweispflichten bestehen

Wenn ein Gastronomiebetrieb, Verein, Veranstalter oder sonstige Organisation die App gegenÃ¼ber eigenen Mitarbeitern, Aushilfen oder Teammitgliedern einsetzt, kann diese Organisation fÃ¼r die konkret eingegebenen Inhalte ganz oder teilweise selbst datenschutzrechtlich verantwortlich sein.

Sie kÃ¶nnen eine erteilte Einwilligung jederzeit mit Wirkung fÃ¼r die Zukunft widerrufen. Die RechtmÃ¤ÃŸigkeit der bis zum Widerruf erfolgten Verarbeitung bleibt hiervon unberÃ¼hrt.

## 6. EmpfÃ¤nger und eingesetzte Dienstleister

Nach dem geprÃ¼ften Code-Stand werden insbesondere folgende externe Dienste genutzt oder eingebunden:

- Firebase Authentication fÃ¼r Login und Benutzerkonten
- Cloud Firestore fÃ¼r Team-, Bestell-, Statistik- und Profildaten
- Firebase Cloud Functions fÃ¼r serverseitige Logik, Abo-Validierung und Datenpflege
- Google Play beziehungsweise Apple App Store fÃ¼r In-App-KÃ¤ufe und Abo-Abwicklung
- Google Sign-In und Sign in with Apple, wenn diese Login-Wege genutzt werden
- System- oder Drittanbieter-Apps, wenn Export-, Ã–ffnen- oder Teilen-Funktionen verwendet werden

Soweit diese Anbieter personenbezogene Daten in Staaten auÃŸerhalb der EuropÃ¤ischen Union oder des EuropÃ¤ischen Wirtschaftsraums verarbeiten, kann eine Ãœbermittlung in Drittstaaten stattfinden. In solchen FÃ¤llen achten wir darauf, dass geeignete Garantien nach Art. 44 ff. DSGVO bestehen, insbesondere AngemessenheitsbeschlÃ¼sse, Standardvertragsklauseln oder sonstige gesetzlich anerkannte Transfermechanismen, soweit diese vom jeweiligen Anbieter bereitgestellt werden.

MaÃŸgeblich fÃ¼r die konkrete Datenverarbeitung durch diese Anbieter bleiben deren Datenschutzinformationen und Vertragsbedingungen.

## 7. Speicherorte und Speicherdauer

### 7.1 Lokale Daten

Lokal gespeicherte Daten bleiben grundsÃ¤tzlich auf Ihrem EndgerÃ¤t gespeichert, bis Sie sie in der App lÃ¶schen, die App deinstallieren oder den lokalen Speicher zurÃ¼cksetzen.

### 7.2 Cloud-Daten fÃ¼r Benutzerprofile und Teambetrieb

Cloud-Daten werden so lange gespeichert, wie dies fÃ¼r den jeweiligen Nutzungszweck erforderlich ist, insbesondere fÃ¼r die laufende Bereitstellung von Team- und Pro-Funktionen.

Aus dem geprÃ¼ften Functions-Code ergeben sich auÃŸerdem folgende automatisch erkennbare Fristen fÃ¼r Teamdaten:

- Teams werden serverseitig geprÃ¼ft und nach 42 Tagen seit Erstellung automatisch geschlossen.
- Geschlossene Teams werden 30 Tage nach dem SchlieÃŸungszeitpunkt rekursiv gelÃ¶scht.
- Offene Join-Requests werden bei TeamschlieÃŸung gelÃ¶scht.
- Inaktive Mitglieder werden serverseitig begrenzt; bei Ãœberschreiten eines Grenzwerts kÃ¶nnen Ã¤ltere inaktive MitgliedseintrÃ¤ge entfernt werden.

### 7.3 Kauf- und Validierungsdaten

Kauf- und Validierungsdaten werden nicht einheitlich, sondern nach ihrer technischen Funktion gespeichert:

- fehlgeschlagene oder technisch auffÃ¤llige Receipt-DatensÃ¤tze werden grundsÃ¤tzlich bis zu 90 Tage gespeichert
- erfolgreich validierte Receipt-DatensÃ¤tze werden grundsÃ¤tzlich bis zu 180 Tage gespeichert
- technische Token-Zuordnungen zur spÃ¤teren Zuordnung von Store-Ereignissen zu Benutzerkonten werden grundsÃ¤tzlich bis zu 365 Tage gespeichert

Diese Fristen dienen der technischen Validierung von KÃ¤ufen, der Missbrauchsabwehr, der ZuordnungsprÃ¼fung, der Bearbeitung typischer SupportfÃ¤lle sowie der sicheren Verarbeitung nachlaufender Store-Ereignisse. MaÃŸgeblich ist jeweils die technische Erforderlichkeit des konkreten Datentyps; Daten werden nicht allein deshalb lÃ¤nger gespeichert, weil der App-Store die Zahlung abgewickelt hat.

Soweit gesetzliche Aufbewahrungspflichten, laufende StreitfÃ¤lle oder sonstige Ã¼berwiegende berechtigte Interessen eine lÃ¤ngere Speicherung erfordern, kann die Speicherung im Einzelfall darÃ¼ber hinausgehen. Im Ãœbrigen sollen diese Daten nach Ablauf der jeweiligen Frist gelÃ¶scht oder soweit praktikabel anonymisiert werden.

## 8. Sicherheit

Der geprÃ¼fte Projektstand verwendet insbesondere folgende Schutzmechanismen:

- Authentifizierung Ã¼ber Firebase Authentication
- Firestore Security Rules zur Begrenzung von Zugriffen auf eigene oder teambezogene Daten
- serverseitige Validierung von Abo-Receipts
- serverseitige Rollen- und StatusprÃ¼fungen fÃ¼r Teamzugriffe
- teilweise serverseitige Steuerung privilegierter Ã„nderungen

Wir weisen darauf hin, dass keine elektronische DatenÃ¼bertragung vollstÃ¤ndig sicher ist. Sie sollten Zugangsdaten vertraulich behandeln und auf EndgerÃ¤ten geeignete SchutzmaÃŸnahmen nutzen.

## 9. Pflicht zur Bereitstellung von Daten

Bestimmte Daten sind erforderlich, damit Cloud-, Team- oder Pro-Funktionen genutzt werden kÃ¶nnen. Ohne Anmeldung, erforderliche Profildaten oder notwendige Team- und Kaufdaten kÃ¶nnen einzelne Funktionen ganz oder teilweise nicht bereitgestellt werden.

## 10. Rechte betroffener Personen

Sie haben nach MaÃŸgabe der gesetzlichen Voraussetzungen insbesondere folgende Rechte:

- Recht auf Auskunft nach Art. 15 DSGVO
- Recht auf Berichtigung nach Art. 16 DSGVO
- Recht auf LÃ¶schung nach Art. 17 DSGVO
- Recht auf EinschrÃ¤nkung der Verarbeitung nach Art. 18 DSGVO
- Recht auf DatenÃ¼bertragbarkeit nach Art. 20 DSGVO
- Recht auf Widerspruch nach Art. 21 DSGVO
- Recht auf Widerruf einer Einwilligung mit Wirkung fÃ¼r die Zukunft
- Recht auf Beschwerde bei einer DatenschutzaufsichtsbehÃ¶rde nach Art. 77 DSGVO

Wenn Sie Rechte geltend machen mÃ¶chten, nutzen Sie bitte die oben genannte Datenschutz-Kontaktadresse.

## 11. Keine automatisierte Entscheidungsfindung

Nach dem derzeit geprÃ¼ften Projektstand findet keine automatisierte Entscheidungsfindung einschlieÃŸlich Profiling im Sinne von Art. 22 DSGVO statt, die Ihnen gegenÃ¼ber rechtliche Wirkung entfaltet oder Sie in Ã¤hnlicher Weise erheblich beeintrÃ¤chtigt.

## 12. Hinweise fÃ¼r gewerbliche oder organisatorische Nutzung

Wenn Sie die App im Rahmen eines Betriebs, Vereins oder einer sonstigen Organisation einsetzen und dabei personenbezogene Daten von Mitarbeitern, Aushilfen, Teammitgliedern, GÃ¤sten oder sonstigen Dritten eintragen, kÃ¶nnen fÃ¼r Sie eigene datenschutzrechtliche Pflichten bestehen. Dazu kÃ¶nnen insbesondere gehÃ¶ren:

- eigene Informationspflichten gegenÃ¼ber betroffenen Personen
- PrÃ¼fung einer passenden Rechtsgrundlage
- interne LÃ¶sch- und Berechtigungskonzepte
- gegebenenfalls vertragliche oder organisatorische Regelungen innerhalb des Betriebs

## 13. Ã„nderungen dieser DatenschutzerklÃ¤rung

Wir kÃ¶nnen diese DatenschutzerklÃ¤rung anpassen, wenn sich App-Funktionen, eingesetzte Dienste, Rechtslagen oder DatenflÃ¼sse Ã¤ndern. Die jeweils aktuelle Fassung sollte in der App, im Store-Listing oder auf einer zugehÃ¶rigen Website bereitgestellt werden.

## 14. Kontakt

Fragen zum Datenschutz kÃ¶nnen an folgende Adresse gerichtet werden:

developer.joviapp@gmail.com


