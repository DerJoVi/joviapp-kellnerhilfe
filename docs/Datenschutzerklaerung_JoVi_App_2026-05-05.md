# Datenschutzerklärung für die JoVi-App

Rechtsversion: 2026-05-11.de-en.v1
Geprüft für App-Version: 2.1.1+261461412

Stand: 05.05.2026

## 1. Verantwortlicher

Verantwortlich für die Verarbeitung personenbezogener Daten im Sinne der Datenschutz-Grundverordnung ist:

Johannes Vilsmeier  
Blütenstr. 11  
71384 Weinstadt  
E-Mail: developer.joviapp@gmail.com  
Datenschutz-Kontakt: developer.joviapp@gmail.com

## 2. Gegenstand der App

Die JoVi-App ist eine App für Bestell-, Team- und Statistikabläufe im Gastronomie-, Veranstaltungs- oder Vereinsumfeld. Nach dem geprüften Projektstand gibt es insbesondere zwei Nutzungsarten:

- lokalen Solo-Betrieb mit Speicherung auf dem Endgerät
- cloudgestützten Team-Betrieb mit Anmeldung, Teamverwaltung, gemeinsamen Bestellungen, Aktivitätsprotokollen, Statistiken und optionalen Pro-Abonnements

## 3. Verarbeitete Daten

### 3.1 Lokal gespeicherte Daten

Im lokalen Betrieb speichert die App Daten insbesondere mit lokalem App-Speicher, Hive und SharedPreferences. Dazu können insbesondere gehören:

- Menüs und Menüpositionen
- Tischbestellungen
- Kassier- und Zahlungsdaten
- Tischlayout und Tischnamen
- App-Einstellungen, Sprache, UI-Skalierung und sonstige Bedienpräferenzen
- lokale Markierungen, Lese- und Ausblendstatus innerhalb der App
- lokale Verlaufsinformationen zu verlassenen Teams

Diese Daten bleiben grundsätzlich auf Ihrem Endgerät, soweit Sie keine Cloud-, Export- oder Teilen-Funktionen nutzen.

### 3.2 Konto- und Anmeldedaten

Bei Nutzung von Cloud- oder Pro-Funktionen verarbeitet die App Authentifizierungs- und Profildaten über Firebase Authentication. Je nach gewählter Anmeldeart können insbesondere verarbeitet werden:

- Benutzer-ID (UID)
- Anzeigename
- E-Mail-Adresse
- Profilbild-URL
- Information, ob ein Konto anonym genutzt wird

Der aktuelle Code sieht Anmeldungen über Google, Apple und eine anonyme Anmeldung für bestimmte Szenarien vor.

### 3.3 Team- und Kollaborationsdaten

Im Team-Modus werden Daten in Firebase Firestore verarbeitet. Dazu gehören je nach Nutzung insbesondere:

- Teamname
- Admin-ID
- Einladungs- oder Join-Code
- Teamstatus, Erstellungs- und Schließungszeitpunkte
- Mitgliederdaten wie Anzeigename, Initialen, Rolle, Mitgliedsstatus und Zeitpunkte von Beitritt oder Austritt
- Join-Requests mit Anzeigename und Antragszeitpunkt
- gemeinsame Menüs
- Tischbestellungen
- Zahlungsdatensätze
- Tischkonfigurationen
- Aktivitäts- und Systemprotokolle mit Text, Zeitstempel, Sendername, Sender-ID und Metadaten
- abgeleitete Tages-Snapshots für Statistikzwecke
- Mitgliedschaftseinträge unter dem jeweiligen Benutzerkonto

Wenn Nutzer in Freitextfeldern oder Teambezeichnungen personenbezogene Angaben eintragen, kann die App auch solche Inhalte verarbeiten.

### 3.4 Abonnement- und Kaufdaten

Bei Nutzung kostenpflichtiger Pro-Funktionen verarbeitet die App abonnementsbezogene Daten. Dazu gehören dem geprüften Code nach insbesondere:

- Produkt-ID des Abonnements
- Plattform des Kaufs
- Kauf-ID oder transaktionsbezogene Kennung
- serverseitige Verifizierungsdaten des jeweiligen Store-Kaufs
- Validierungsstatus und Validierungszeitpunkt
- Ablaufdatum des Abonnements
- Zuordnung eines Kauf-Tokens zu einer Benutzer-ID
- Pro-Status des Benutzerkontos

Die eigentliche Zahlungsabwicklung erfolgt über den jeweiligen App-Store. Vollständige Zahlungsdaten wie Kreditkarten- oder Bankdaten werden nach dem erkennbaren Projektstand nicht von der App selbst gespeichert.

Unabhängig davon verarbeitet die App eigene abonnementsbezogene Nachweis-, Prüf- und Statusdaten, soweit dies für die technische Validierung eines Kaufs, die Missbrauchsabwehr, die Zuordnung eines Kaufs zu einem Benutzerkonto und die Freischaltung oder Einschränkung von Pro-Funktionen erforderlich ist. Dazu können insbesondere in Firestore eingereichte Kaufnachweise, serverseitige Prüfergebnisse, Token-Zuordnungen und Statusfelder zum Pro-Abonnement gehören.

Nach dem aktuellen technischen Stand werden diese Datenarten mit unterschiedlichen Löschfristen behandelt. Kurzlebige technische Fehler- und Prüfdatensätze zu eingereichten Kaufnachweisen werden kürzer aufbewahrt als erfolgreich validierte Kaufnachweise. Reine Token-Zuordnungen zur technischen Zuordnung späterer Store-Ereignisse können länger gespeichert werden als die eigentlichen Receipt-Datensätze.

### 3.5 Export-, Import- und Freigabedaten

Die App bietet Export-, Import-, Download-, Öffnen- und Teilen-Funktionen. Dabei können insbesondere verarbeitet oder an von Ihnen ausgewählte Ziele übergeben werden:

- Menüdateien im .jovi-Format
- CSV-, HTML- und PDF-Exporte
- Statistikdateien
- Inhalte aus lokalen oder cloudbasierten Datenbeständen

Wenn Sie eine Teilen-, Öffnen- oder Speichern-Funktion verwenden, werden Daten an die von Ihnen ausgewählte Ziel-App, Dateiablage oder Systemfunktion übergeben. Ab diesem Zeitpunkt gelten zusätzlich deren Datenschutzbedingungen.

### 3.6 Kamera- und Scan-Funktionen

Der aktuelle Code verwendet eine Scanner-Funktion für QR- oder kameragestützte Vorgänge. Die Kamera wird nur genutzt, wenn Sie die entsprechende Funktion aktiv aufrufen.

### 3.7 Technische und betriebliche Daten

Zur Bereitstellung der App können außerdem technische Metadaten verarbeitet werden, insbesondere:

- Plattform und Betriebssystemkontext
- App-Version und Build-Nummer
- Zeitstempel von Vorgängen
- Fehler- und Statusinformationen innerhalb der App- und Cloud-Abläufe
- Berechtigungs- und Sicherheitsstatus bei Zugriffen auf Cloud-Daten

Aus dem geprüften Code ergibt sich kein eigenständiger Einsatz von Werbetracking, Werbe-SDKs oder klassischem Nutzerprofiling.

## 4. Zwecke der Verarbeitung

Wir verarbeiten Daten insbesondere zu folgenden Zwecken:

- Bereitstellung der App-Funktionen
- Speicherung und Synchronisierung von Bestellungen, Menüs, Teamdaten und Statistiken
- Benutzeranmeldung und Kontoverwaltung
- Teamverwaltung und Nachvollziehbarkeit von Team-Aktivitäten
- Prüfung und Durchsetzung von Berechtigungen und Sicherheitsregeln
- Abwicklung und Validierung von Pro-Abonnements
- Export, Import, Öffnen und Teilen von Inhalten auf Wunsch der Nutzer
- Fehleranalyse, Missbrauchsvermeidung und technische Stabilität

## 5. Rechtsgrundlagen

Soweit die DSGVO anwendbar ist, stützen wir die Verarbeitung insbesondere auf folgende Rechtsgrundlagen:

- Art. 6 Abs. 1 lit. b DSGVO für die Bereitstellung vertraglich oder vorvertraglich angefragter App-Funktionen
- Art. 6 Abs. 1 lit. f DSGVO für Sicherheits-, Missbrauchsabwehr-, Stabilitäts- und Verwaltungszwecke
- Art. 6 Abs. 1 lit. a DSGVO, soweit Sie freiwillig Funktionen wie externe Freigaben, Kameraeinsatz oder bestimmte Login-Verfahren nutzen
- Art. 6 Abs. 1 lit. c DSGVO, soweit rechtliche Aufbewahrungs- oder Nachweispflichten bestehen

Wenn ein Gastronomiebetrieb, Verein, Veranstalter oder sonstige Organisation die App gegenüber eigenen Mitarbeitern, Aushilfen oder Teammitgliedern einsetzt, kann diese Organisation für die konkret eingegebenen Inhalte ganz oder teilweise selbst datenschutzrechtlich verantwortlich sein.

Sie können eine erteilte Einwilligung jederzeit mit Wirkung für die Zukunft widerrufen. Die Rechtmäßigkeit der bis zum Widerruf erfolgten Verarbeitung bleibt hiervon unberührt.

## 6. Empfänger und eingesetzte Dienstleister

Nach dem geprüften Code-Stand werden insbesondere folgende externe Dienste genutzt oder eingebunden:

- Firebase Authentication für Login und Benutzerkonten
- Cloud Firestore für Team-, Bestell-, Statistik- und Profildaten
- Firebase Cloud Functions für serverseitige Logik, Abo-Validierung und Datenpflege
- Google Play beziehungsweise Apple App Store für In-App-Käufe und Abo-Abwicklung
- Google Sign-In und Sign in with Apple, wenn diese Login-Wege genutzt werden
- System- oder Drittanbieter-Apps, wenn Export-, Öffnen- oder Teilen-Funktionen verwendet werden

Soweit diese Anbieter personenbezogene Daten in Staaten außerhalb der Europäischen Union oder des Europäischen Wirtschaftsraums verarbeiten, kann eine Übermittlung in Drittstaaten stattfinden. In solchen Fällen achten wir darauf, dass geeignete Garantien nach Art. 44 ff. DSGVO bestehen, insbesondere Angemessenheitsbeschlüsse, Standardvertragsklauseln oder sonstige gesetzlich anerkannte Transfermechanismen, soweit diese vom jeweiligen Anbieter bereitgestellt werden.

Maßgeblich für die konkrete Datenverarbeitung durch diese Anbieter bleiben deren Datenschutzinformationen und Vertragsbedingungen.

## 7. Speicherorte und Speicherdauer

### 7.1 Lokale Daten

Lokal gespeicherte Daten bleiben grundsätzlich auf Ihrem Endgerät gespeichert, bis Sie sie in der App löschen, die App deinstallieren oder den lokalen Speicher zurücksetzen.

### 7.2 Cloud-Daten für Benutzerprofile und Teambetrieb

Cloud-Daten werden so lange gespeichert, wie dies für den jeweiligen Nutzungszweck erforderlich ist, insbesondere für die laufende Bereitstellung von Team- und Pro-Funktionen.

Aus dem geprüften Functions-Code ergeben sich außerdem folgende automatisch erkennbare Fristen für Teamdaten:

- Teams werden serverseitig geprüft und nach 42 Tagen seit Erstellung automatisch geschlossen.
- Geschlossene Teams werden 30 Tage nach dem Schließungszeitpunkt rekursiv gelöscht.
- Offene Join-Requests werden bei Teamschließung gelöscht.
- Inaktive Mitglieder werden serverseitig begrenzt; bei Überschreiten eines Grenzwerts können ältere inaktive Mitgliedseinträge entfernt werden.

### 7.3 Kauf- und Validierungsdaten

Kauf- und Validierungsdaten werden nicht einheitlich, sondern nach ihrer technischen Funktion gespeichert:

- fehlgeschlagene oder technisch auffällige Receipt-Datensätze werden grundsätzlich bis zu 90 Tage gespeichert
- erfolgreich validierte Receipt-Datensätze werden grundsätzlich bis zu 180 Tage gespeichert
- technische Token-Zuordnungen zur späteren Zuordnung von Store-Ereignissen zu Benutzerkonten werden grundsätzlich bis zu 365 Tage gespeichert

Diese Fristen dienen der technischen Validierung von Käufen, der Missbrauchsabwehr, der Zuordnungsprüfung, der Bearbeitung typischer Supportfälle sowie der sicheren Verarbeitung nachlaufender Store-Ereignisse. Maßgeblich ist jeweils die technische Erforderlichkeit des konkreten Datentyps; Daten werden nicht allein deshalb länger gespeichert, weil der App-Store die Zahlung abgewickelt hat.

Soweit gesetzliche Aufbewahrungspflichten, laufende Streitfälle oder sonstige überwiegende berechtigte Interessen eine längere Speicherung erfordern, kann die Speicherung im Einzelfall darüber hinausgehen. Im Übrigen sollen diese Daten nach Ablauf der jeweiligen Frist gelöscht oder soweit praktikabel anonymisiert werden.

## 8. Sicherheit

Der geprüfte Projektstand verwendet insbesondere folgende Schutzmechanismen:

- Authentifizierung über Firebase Authentication
- Firestore Security Rules zur Begrenzung von Zugriffen auf eigene oder teambezogene Daten
- serverseitige Validierung von Abo-Receipts
- serverseitige Rollen- und Statusprüfungen für Teamzugriffe
- teilweise serverseitige Steuerung privilegierter Änderungen

Wir weisen darauf hin, dass keine elektronische Datenübertragung vollständig sicher ist. Sie sollten Zugangsdaten vertraulich behandeln und auf Endgeräten geeignete Schutzmaßnahmen nutzen.

## 9. Pflicht zur Bereitstellung von Daten

Bestimmte Daten sind erforderlich, damit Cloud-, Team- oder Pro-Funktionen genutzt werden können. Ohne Anmeldung, erforderliche Profildaten oder notwendige Team- und Kaufdaten können einzelne Funktionen ganz oder teilweise nicht bereitgestellt werden.

## 10. Rechte betroffener Personen

Sie haben nach Maßgabe der gesetzlichen Voraussetzungen insbesondere folgende Rechte:

- Recht auf Auskunft nach Art. 15 DSGVO
- Recht auf Berichtigung nach Art. 16 DSGVO
- Recht auf Löschung nach Art. 17 DSGVO
- Recht auf Einschränkung der Verarbeitung nach Art. 18 DSGVO
- Recht auf Datenübertragbarkeit nach Art. 20 DSGVO
- Recht auf Widerspruch nach Art. 21 DSGVO
- Recht auf Widerruf einer Einwilligung mit Wirkung für die Zukunft
- Recht auf Beschwerde bei einer Datenschutzaufsichtsbehörde nach Art. 77 DSGVO

Wenn Sie Rechte geltend machen möchten, nutzen Sie bitte die oben genannte Datenschutz-Kontaktadresse.

## 11. Keine automatisierte Entscheidungsfindung

Nach dem derzeit geprüften Projektstand findet keine automatisierte Entscheidungsfindung einschließlich Profiling im Sinne von Art. 22 DSGVO statt, die Ihnen gegenüber rechtliche Wirkung entfaltet oder Sie in ähnlicher Weise erheblich beeinträchtigt.

## 12. Hinweise für gewerbliche oder organisatorische Nutzung

Wenn Sie die App im Rahmen eines Betriebs, Vereins oder einer sonstigen Organisation einsetzen und dabei personenbezogene Daten von Mitarbeitern, Aushilfen, Teammitgliedern, Gästen oder sonstigen Dritten eintragen, können für Sie eigene datenschutzrechtliche Pflichten bestehen. Dazu können insbesondere gehören:

- eigene Informationspflichten gegenüber betroffenen Personen
- Prüfung einer passenden Rechtsgrundlage
- interne Lösch- und Berechtigungskonzepte
- gegebenenfalls vertragliche oder organisatorische Regelungen innerhalb des Betriebs

## 13. Änderungen dieser Datenschutzerklärung

Wir können diese Datenschutzerklärung anpassen, wenn sich App-Funktionen, eingesetzte Dienste, Rechtslagen oder Datenflüsse ändern. Die jeweils aktuelle Fassung sollte in der App, im Store-Listing oder auf einer zugehörigen Website bereitgestellt werden.

## 14. Kontakt

Fragen zum Datenschutz können an folgende Adresse gerichtet werden:

developer.joviapp@gmail.com
