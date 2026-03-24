# joviapp-kellnerhilfe
JoVi App Kellnerhilfe
[DATENSCHUTZERKLAERUNG.md](https://github.com/user-attachments/files/26197708/DATENSCHUTZERKLAERUNG.md)
# Datenschutzerklärung – JoVi-App Kellnerhilfe

**Stand: März 2026**
**Version der App: 1.3.3**

---

## 1. Verantwortlicher

Verantwortlich für die Datenverarbeitung im Sinne der Datenschutz-Grundverordnung (DSGVO) ist:

**JoVi Labs**
*Johannes Vilsmeier*
71384 Weinstadt
developer.joviapp@gmail.com

---

## 2. Überblick – Das Wichtigste auf einen Blick

Die JoVi-App Kellnerhilfe wurde nach dem Grundsatz **„Privacy by Design"** entwickelt:

- **Alle Daten bleiben auf Ihrem Gerät.** Es werden keine Daten an Server, Cloud-Dienste oder Dritte übertragen.
- **Keine Registrierung erforderlich.** Die App erfordert kein Benutzerkonto.
- **Keine Tracking- oder Analyse-Dienste.** Es werden keine Analyse-, Werbe- oder Tracking-SDKs eingesetzt.
- **Keine Internetverbindung erforderlich.** Die App funktioniert vollständig offline.
- **Minimale Berechtigungen.** Die App fordert nur Berechtigungen an, die für die jeweilige Funktion unbedingt notwendig sind.

---

## 3. Welche Daten werden verarbeitet?

### 3.1 Lokal gespeicherte Daten

Die folgenden Daten werden **ausschließlich lokal** auf Ihrem Gerät gespeichert und verlassen dieses zu keinem Zeitpunkt automatisch:

| Datenkategorie | Beschreibung | Speicherort |
|----------------|-------------|-------------|
| **Speisekarten/Menüs** | Von Ihnen erstellte Menüs mit Artikelnamen und Preisen | Hive-Datenbank (lokal) |
| **Bestellungen** | Aktive Bestellungen pro Tischnummer mit Artikeln und Mengen | Hive-Datenbank (lokal) |
| **Zahlungseinträge** | Abgerechnete Bestellungen mit Datum, Uhrzeit, Tischnummer, Betrag und optionaler Notiz | Hive-Datenbank (lokal) |
| **App-Einstellungen** | Gewählte Sprache und Währung | SharedPreferences (lokal) |
| **Fehlerprotokolle** | Technische Fehlermeldungen der App (max. 500 Einträge) | Hive-Datenbank (lokal) |

### 3.2 Keine personenbezogenen Daten

Die App erhebt und verarbeitet **keine personenbezogenen Daten** im Sinne der DSGVO. Insbesondere werden folgende Daten **nicht** erhoben:

- Keine Namen, Adressen oder Kontaktdaten von Nutzern oder Gästen
- Keine E-Mail-Adressen oder Telefonnummern
- Keine Standortdaten oder GPS-Daten
- Keine Geräte-IDs, Werbe-IDs oder eindeutige Kennungen
- Keine IP-Adressen
- Keine Nutzungsstatistiken oder Verhaltensdaten
- Keine biometrischen Daten

### 3.3 Hinweis zu frei eingegebenen Texten

In optionalen Notizfeldern (z. B. bei Zahlungseinträgen) können Sie frei Text eingeben. Wenn Sie dort personenbezogene Daten eintragen (z. B. Gästenamen), liegt die Verantwortung für die Verarbeitung dieser Daten bei Ihnen als Nutzer.

---

## 4. Berechtigungen

Die App fordert folgende Geräteberechtigungen an – **nur bei Bedarf** und **nur nach Ihrer Zustimmung**:

### 4.1 Kamera

- **Zweck:** Scannen von QR-Codes zum Importieren von Speisekarten
- **Wann:** Nur wenn Sie die QR-Code-Scan-Funktion aktiv nutzen
- **Datenverarbeitung:** Das Kamerabild wird ausschließlich lokal verarbeitet, um den QR-Code zu dekodieren. Es werden keine Bilder gespeichert oder übertragen.
- **Bibliothek:** `mobile_scanner` (lokale Verarbeitung)

### 4.2 Dateizugriff / Speicher

- **Zweck:** Speichern und Laden von Menü-Dateien (.jovi-Format) sowie Export von Statistiken (PDF/HTML)
- **Wann:** Nur wenn Sie die Import-/Export-Funktion aktiv nutzen
- **Datenverarbeitung:** Es werden nur die von Ihnen gewählten Dateien gelesen oder geschrieben. Die App greift nicht eigenständig auf andere Dateien zu.
- **Bibliothek:** `file_picker`, `path_provider`, `share_plus`

---

## 5. Datenübertragung

### 5.1 Keine automatische Datenübertragung

Die App sendet **keine Daten** an Server, Cloud-Dienste, Analyseplattformen oder sonstige Dritte. Es findet kein automatischer Datenverkehr statt.

### 5.2 Vom Nutzer initiierter Datenaustausch

Folgende Funktionen ermöglichen einen **vom Nutzer aktiv ausgelösten** Datenaustausch:

| Funktion | Beschreibung | Übertragene Daten |
|----------|-------------|-------------------|
| **Menü-Export (.jovi)** | Speichert ein Menü als Datei auf dem Gerät oder teilt es über andere Apps | Menüname, Artikelnamen, Preise, Kategorien |
| **QR-Code-Sharing** | Generiert einen QR-Code mit Menüdaten zum Anzeigen/Teilen | Menüname, Artikelnamen, Preise, Kategorien (in kodierter Form) |
| **Statistik-Export** | Exportiert Tagesabrechnungen als PDF oder HTML | Datum, Tischnummern, Beträge, Artikel, optionale Notizen |

Hinweis: Bei Nutzung der Teilen-Funktion (Share) werden die Daten an die vom Nutzer gewählte Ziel-App übergeben (z. B. E-Mail, Messenger). Die Datenschutzbestimmungen der jeweiligen Ziel-App gelten ab diesem Zeitpunkt.

### 5.3 Keine Drittanbieter-SDKs mit Datenübertragung

Die App verwendet **keine** der folgenden Dienste:
- Keine Analyse-Tools (Google Analytics, Firebase Analytics, Mixpanel o. Ä.)
- Keine Crash-Reporting-Dienste (Crashlytics, Sentry o. Ä.)
- Keine Werbedienste (Google Ads, Facebook Ads o. Ä.)
- Keine Push-Notification-Dienste
- Keine Social-Media-SDKs
- Keine Cloud-Speicherdienste

---

## 6. Drittanbieter-Bibliotheken

Die App verwendet folgende Open-Source-Bibliotheken. Keine dieser Bibliotheken überträgt Daten an Dritte:

| Bibliothek | Zweck | Datenverarbeitung |
|------------|-------|-------------------|
| `hive` / `hive_flutter` | Lokale Datenbank | Rein lokal, keine Netzwerkzugriffe |
| `shared_preferences` | Einstellungen speichern | Rein lokal |
| `mobile_scanner` | QR-Code-Scanning | Lokale Kameraverarbeitung, keine Datenübertragung |
| `qr_flutter` | QR-Code-Generierung | Rein lokal, keine Netzwerkzugriffe |
| `file_picker` | Dateiauswahl | Zugriff auf vom Nutzer gewählte Dateien |
| `path_provider` | App-Verzeichnisse | Rein lokal |
| `share_plus` | Teilen-Funktion | Übergibt Daten an vom Nutzer gewählte Ziel-App |
| `pdf` | PDF-Generierung | Rein lokal |
| `uuid` | Eindeutige IDs | Lokale Generierung, keine Netzwerkzugriffe |
| `crypto` | Hashing (MD5) | Lokale Berechnung für Artikel-IDs |
| `image` | Bildverarbeitung | Rein lokal |
| `intl` | Internationalisierung | Rein lokal |
| `package_info_plus` | App-Versionsinformation | Liest lokale App-Metadaten |

---

## 7. Datensicherheit

### 7.1 Lokale Speicherung

Alle Daten werden in der **Hive-Datenbank** im geschützten App-Verzeichnis des Betriebssystems gespeichert. Der Zugriff auf diese Daten ist durch die Sandbox-Mechanismen des jeweiligen Betriebssystems (Android/iOS) geschützt.

### 7.2 Keine Verschlüsselung der lokalen Datenbank

Die lokale Hive-Datenbank ist **nicht zusätzlich verschlüsselt**. Der Schutz der Daten basiert auf der Betriebssystem-Sandbox und der Geräteverschlüsselung Ihres Endgeräts. Wir empfehlen:

- Aktivieren Sie die **Geräteverschlüsselung** (bei den meisten modernen Geräten standardmäßig aktiv)
- Verwenden Sie eine **Bildschirmsperre** (PIN, Muster, Fingerabdruck oder Gesichtserkennung)
- Halten Sie das **Betriebssystem** Ihres Geräts aktuell

### 7.3 Export-Dateien

Exportierte .jovi-Dateien und PDF/HTML-Berichte werden **unverschlüsselt** gespeichert. Wenn diese Dateien sensible Preisinformationen enthalten, behandeln Sie sie entsprechend vertraulich.

---

## 8. Speicherdauer und Löschung

### 8.1 Aufbewahrung

| Daten | Speicherdauer |
|-------|--------------|
| Menüs | Bis zur Löschung durch den Nutzer |
| Aktive Bestellungen | Bis zur Abrechnung oder manuellen Löschung |
| Zahlungseinträge | Bis zur Löschung durch den Nutzer (tagesweise oder komplett) |
| Fehlerprotokolle | Automatische Bereinigung ab 500 Einträgen (älteste werden gelöscht) |
| App-Einstellungen | Bis zur Deinstallation der App |

### 8.2 Löschung

Sie können Ihre Daten jederzeit löschen:

- **Einzelnes Menü löschen:** In der Menü-Verwaltung
- **Tagesstatistik löschen:** In den Einstellungen (für ein bestimmtes Datum)
- **Alle Statistiken löschen:** In den Einstellungen
- **Alle App-Daten löschen:** Über die Systemeinstellungen Ihres Geräts (App-Daten löschen) oder durch Deinstallation der App

Bei Deinstallation der App werden **alle lokal gespeicherten Daten unwiderruflich gelöscht**.

---

## 9. Rechtsgrundlage

Da die App keine personenbezogenen Daten erhebt oder verarbeitet, entfällt die Notwendigkeit einer Rechtsgrundlage nach Art. 6 DSGVO für die reguläre Nutzung der App.

Sofern Sie in optionalen Freitextfeldern personenbezogene Daten eingeben, erfolgt dies auf Basis Ihrer Einwilligung (Art. 6 Abs. 1 lit. a DSGVO) bzw. zur Wahrung Ihrer berechtigten Interessen als Gewerbetreibender (Art. 6 Abs. 1 lit. f DSGVO).

---

## 10. Ihre Rechte

Obwohl die App selbst keine personenbezogenen Daten verarbeitet, stehen Ihnen im Rahmen der DSGVO grundsätzlich folgende Rechte zu:

- **Recht auf Auskunft** (Art. 15 DSGVO)
- **Recht auf Berichtigung** (Art. 16 DSGVO)
- **Recht auf Löschung** (Art. 17 DSGVO)
- **Recht auf Einschränkung der Verarbeitung** (Art. 18 DSGVO)
- **Recht auf Datenübertragbarkeit** (Art. 20 DSGVO)
- **Recht auf Widerspruch** (Art. 21 DSGVO)

Für die Ausübung dieser Rechte wenden Sie sich bitte an den oben genannten Verantwortlichen.

Sie haben zudem das Recht, eine **Beschwerde bei einer Aufsichtsbehörde** einzureichen (Art. 77 DSGVO).

---

## 11. Kinder und Jugendliche

Die App richtet sich an gewerbliche Nutzer im Gastronomiebereich und ist nicht für die Nutzung durch Kinder unter 16 Jahren vorgesehen. Es werden keine Daten von Kindern erhoben.

---

## 12. Hinweise für gewerbliche Nutzer

Wenn Sie die JoVi-App im gewerblichen Kontext einsetzen (z. B. als Kellner, Gastronom oder Festwirt), beachten Sie bitte:

- **Sie sind selbst verantwortlich** für personenbezogene Daten, die Sie in Freitextfeldern der App eingeben.
- Bei der Verwendung der **Export-Funktionen** (Teilen von Menüs, Statistik-Export) verlassen Daten das geschützte App-Verzeichnis. Stellen Sie sicher, dass der Empfänger vertrauenswürdig ist.
- Wenn Sie die App im Rahmen Ihres Gewerbes nutzen und dabei personenbezogene Daten verarbeiten, können **eigene datenschutzrechtliche Pflichten** für Sie gelten (z. B. Verarbeitungsverzeichnis, Informationspflichten gegenüber Ihren Gästen).
- Bewahren Sie exportierte Dateien (.jovi, PDF, HTML) gemäß den geltenden **Aufbewahrungsfristen** sicher auf.

---

## 13. Änderungen dieser Datenschutzerklärung

Wir behalten uns vor, diese Datenschutzerklärung bei Bedarf anzupassen, insbesondere bei Änderungen der App-Funktionen oder bei Änderungen der rechtlichen Anforderungen. Die aktuelle Version wird stets in der App und auf der App-Seite im jeweiligen Store verfügbar sein.

---

## 14. Kontakt

Bei Fragen zum Datenschutz oder zur Ausübung Ihrer Rechte wenden Sie sich bitte an:

**JoVi Labs**
JoVi Labs Johannes Vilsmeier 71384 Weinstadt 

E-Mail: *developer.joviapp@gmail.com*

---

*Diese Datenschutzerklärung bezieht sich auf Version 1.3.3 der JoVi-App Kellnerhilfe. Stand: März 2026.*
