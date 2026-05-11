# Datenschutzerklärung für die JoVi-App

> Entwurf auf Basis des aktuellen Projektstands vom 05.05.2026.
> Dieser Text bildet die im Code erkennbaren Datenverarbeitungen ab. Vor Veröffentlichung sollten die markierten Platzhalter durch Ihre echten Anbieter- und Kontaktdaten ersetzt und rechtlich geprüft werden.

## 1. Verantwortlicher

Verantwortlich für die Verarbeitung personenbezogener Daten im Sinne der DSGVO ist nach aktuellem Projektstand:

[PLATZHALTER: Name der verantwortlichen Person oder Firma]  
E-Mail: [PLATZHALTER: allgemeine Kontakt-E-Mail]  
Datenschutz-Kontakt: [PLATZHALTER: Datenschutz-E-Mail]  
Anschrift: [PLATZHALTER: vollständige ladungsfähige Anschrift]  

Sofern ein Datenschutzbeauftragter bestellt ist, kann dieser unter folgenden Kontaktdaten erreicht werden:

[PLATZHALTER: Datenschutzbeauftragter oder Vermerk, dass keiner bestellt ist]

Bitte vor Veröffentlichung ergänzen:
- vollständige ladungsfähige Anschrift mit Straße und Hausnummer
- gegebenenfalls Rechtsform oder Firmenbezeichnung
- gegebenenfalls Impressums-URL
- gegebenenfalls Datenschutzbeauftragter mit Kontaktdaten

## 2. Worum es in der App geht

Die JoVi-App ist eine App für Bestell-, Team- und Statistikabläufe im Gastronomie- und Veranstaltungsumfeld. Der Code zeigt zwei Nutzungsarten:

- lokalen Solo-Betrieb mit Speicherung auf dem Gerät
- cloudgestützten Team-Betrieb mit Anmeldung, Teamverwaltung, gemeinsamen Bestellungen, Aktivitätsprotokollen, Statistiken und optionalen Pro-Abonnements

## 3. Welche Daten wir verarbeiten

### 3.1 Lokal auf dem Endgerät gespeicherte Daten

Im lokalen Betrieb speichert die App Daten insbesondere in lokalem App-Speicher mittels Hive und SharedPreferences. Dazu können insbesondere gehören:

- Menüs und Menüpositionen
- Tischbestellungen
- Kassier- und Zahlungsdaten
- Tischlayout und Tischnamen
- App-Einstellungen, Sprache, UI-Skalierung und sonstige Bedienpräferenzen
- lokale Markierungen, Lese- und Ausblendstatus innerhalb der App
- lokale Verlaufsinformationen zu verlassenen Teams

Diese Daten bleiben grundsätzlich auf Ihrem Endgerät, soweit Sie keine Cloud- oder Teilen-Funktionen nutzen.

### 3.2 Konto- und Anmeldedaten

Bei Nutzung von Cloud- oder Pro-Funktionen verarbeitet die App Authentifizierungs- und Profildaten über Firebase Authentication. Je nach gewählter Anmeldeart können insbesondere verarbeitet werden:

- Benutzer-ID (UID)
- Anzeigename
- E-Mail-Adresse
- Profilbild-URL
- Information, ob ein Konto anonym genutzt wird

Der Code sieht Anmeldungen über Google, Apple und anonyme Anmeldung vor.

### 3.3 Team- und Kollaborationsdaten

Im Team-Modus werden Daten in Firebase Firestore verarbeitet. Dazu gehören je nach Nutzung insbesondere:

- Teamname
- Admin-ID
- Einladungs- bzw. Join-Code
- Teamstatus, Erstellungs- und Schließungszeitpunkte
- Mitgliederdaten wie Anzeigename, Initialen, Rolle, Mitgliedsstatus und Zeitpunkte von Beitritt bzw. Austritt
- Join-Requests mit Anzeigename und Antragszeitpunkt
- gemeinsame Menüs
- Tischbestellungen
- Zahlungsdatensätze
- Tischkonfigurationen
- Aktivitäts- und Systemprotokolle mit Text, Zeitstempel, Sendername, Sender-ID und Metadaten
- abgeleitete Tages-Snapshots für Statistikzwecke
- Mitgliedschaftseinträge unter dem jeweiligen Benutzerkonto

Bitte beachten Sie: Inhalte, die Sie oder andere Teammitglieder selbst eintragen, können personenbezogene Daten enthalten, wenn dort etwa Klarnamen, Notizen oder sonstige personenbeziehbare Inhalte verwendet werden.

### 3.4 Abonnement- und Kaufdaten

Bei Nutzung kostenpflichtiger Pro-Funktionen verarbeitet die App abonnementsbezogene Daten. Dem Code nach gehören dazu insbesondere:

- Produkt-ID des Abonnements, zum Beispiel monatlich oder jährlich
- Plattform des Kaufs
- Kauf-ID oder transaktionsbezogene Kennung
- serverseitige Verifizierungsdaten des jeweiligen Store-Kaufs
- Validierungsstatus und Validierungszeitpunkt
- Ablaufdatum des Abonnements
- Zuordnung eines Kauf-Tokens zu einer Benutzer-ID
- Pro-Status des Benutzerkontos

Die eigentliche Zahlungsabwicklung erfolgt über den jeweiligen App-Store. Vollständige Zahlungsdaten wie Kreditkarten- oder Bankdaten werden nach dem erkennbaren Projektstand nicht von der App selbst gespeichert.

Unabhängig davon verarbeitet die App eigene abonnementsbezogene Nachweis-, Prüf- und Statusdaten, soweit dies für die technische Validierung eines Kaufs, die Missbrauchsabwehr, die Zuordnung eines Kaufs zu einem Benutzerkonto und die Freischaltung oder Einschränkung von Pro-Funktionen erforderlich ist. Dazu können insbesondere in Firestore eingereichte Kaufnachweise, serverseitige Prüfergebnisse, Token-Zuordnungen und Statusfelder zum Pro-Abonnement gehören.

### 3.5 Export-, Import- und Freigabedaten

Die App bietet Export-, Import-, Download-, Öffnen- und Teilen-Funktionen. Dabei können insbesondere verarbeitet oder an von Ihnen ausgewählte Ziele übergeben werden:

- Menüdateien im .jovi-Format
- CSV-, HTML- und PDF-Exporte
- Statistikdateien
- Inhalte aus lokalen oder cloudbasierten Datenbeständen

Wenn Sie eine Teilen-, Öffnen- oder Speichern-Funktion verwenden, werden Daten an die von Ihnen ausgewählte Ziel-App, Dateiablage oder Systemfunktion übergeben. Ab diesem Zeitpunkt gelten zusätzlich deren Datenschutzbedingungen.

### 3.6 Kamera- und Scan-Funktionen

Der Code verwendet eine Scanner-Funktion für QR- bzw. kameragestützte Vorgänge. Die Kamera wird nur genutzt, wenn Sie die entsprechende Scan-Funktion aktiv aufrufen.

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

Nach dem Code-Stand werden insbesondere folgende externe Dienste genutzt oder eingebunden:

- Firebase Authentication für Login und Benutzerkonten
- Cloud Firestore für Team-, Bestell-, Statistik- und Profildaten
- Firebase Cloud Functions für serverseitige Logik, Abo-Validierung und Datenpflege
- Google Play bzw. Apple App Store für In-App-Käufe und Abo-Abwicklung
- Google Sign-In und Sign in with Apple, wenn Sie diese Login-Wege nutzen
- System- oder Drittanbieter-Apps, wenn Sie Export-, Öffnen- oder Teilen-Funktionen verwenden

Soweit diese Anbieter personenbezogene Daten in Staaten außerhalb der Europäischen Union oder des Europäischen Wirtschaftsraums verarbeiten, kann eine Übermittlung in Drittstaaten stattfinden. In solchen Fällen achten wir darauf, dass geeignete Garantien nach Art. 44 ff. DSGVO bestehen, insbesondere Angemessenheitsbeschlüsse, Standardvertragsklauseln oder sonstige gesetzlich anerkannte Transfermechanismen, soweit diese vom jeweiligen Anbieter bereitgestellt werden.

Maßgeblich für die konkrete Datenverarbeitung durch diese Anbieter bleiben deren Datenschutzinformationen und Vertragsbedingungen.

## 7. Speicherorte und Speicherdauer

### 7.1 Lokale Daten

Lokal gespeicherte Daten bleiben grundsätzlich auf Ihrem Endgerät gespeichert, bis Sie sie in der App löschen, die App deinstallieren oder den lokalen Speicher zurücksetzen.

### 7.2 Cloud-Daten für Benutzerprofile und Teambetrieb

Cloud-Daten werden so lange gespeichert, wie dies für den jeweiligen Nutzungszweck erforderlich ist, insbesondere für die laufende Bereitstellung von Team- und Pro-Funktionen.

Aus dem geprüften Functions-Code ergeben sich außerdem folgende automatische Fristen für Teamdaten:

- Teams werden täglich serverseitig geprüft und nach 42 Tagen seit Erstellung automatisch geschlossen.
- Geschlossene Teams werden 30 Tage nach dem Schließungszeitpunkt rekursiv gelöscht.
- Offene Join-Requests werden bei Teamschließung gelöscht.
- Inaktive Mitglieder werden serverseitig begrenzt; bei Überschreiten eines Grenzwerts können ältere inaktive Mitgliedseinträge entfernt werden.

### 7.3 Kauf- und Validierungsdaten

Kaufbelege und Verifizierungsdaten werden mindestens so lange gespeichert, wie sie für die Abo-Validierung, Missbrauchsabwehr, Zuordnungsprüfung und technische Nachvollziehbarkeit erforderlich sind.

Soweit keine längeren gesetzlichen Aufbewahrungspflichten oder berechtigten Interessen entgegenstehen, sollten diese Daten nach einer intern festgelegten Löschfrist gelöscht oder anonymisiert werden. Eine solche Frist sollte vor Veröffentlichung organisatorisch festgelegt werden.

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

## 10. Ihre Rechte

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

Fragen zum Datenschutz können Sie derzeit an folgende Adresse richten:

[PLATZHALTER: Datenschutz-E-Mail]

---

Stand dieses Entwurfs: 05.05.2026