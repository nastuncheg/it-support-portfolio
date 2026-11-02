# Verdacht auf Umgehung einer DLP-Richtlinie beim Versand von Kundendaten

**Ticket-Typ:** Security-Related Service Request  
**Priorität:** Hoch  
**Systeme:** Microsoft 365, SharePoint, Data Loss Prevention (DLP), Conditional Access  
**Status:** Training Simulation, eskaliert

## 1. Problembeschreibung

Ein Mitarbeiter möchte eine Excel-Datei mit etwa 2.000 Kundendatensätzen, einschließlich Adressen und Telefonnummern, an seine private Gmail-Adresse senden.

Die E-Mail wird durch eine Sicherheitsrichtlinie blockiert. Der Mitarbeiter bittet den IT-Support darum, die Blockierung kurzfristig aufzuheben, da er die Datei am Abend von zu Hause aus bearbeiten muss. Die Abgabe ist für den nächsten Tag geplant.

## 2. Ersteinschätzung

Es handelt sich um eine sicherheitsrelevante Anfrage mit möglichem Data-Loss-Prevention-(DLP)-Vorfall.

Die Datei enthält personenbezogene Daten. Eine Übertragung an ein privates E-Mail-Konto kann ein Risiko für Datenschutz und Informationssicherheit darstellen.

Mögliche Ursachen und Risiken:

- Eine DLP-Richtlinie erkennt personenbezogene Daten und verhindert deren Übertragung außerhalb der Organisation.
- Der Mitarbeiter kennt möglicherweise die geltenden Sicherheitsrichtlinien nicht und versucht, eine praktische Lösung für die Arbeit von zu Hause zu finden.
- Es könnte sich um einen Versuch handeln, Unternehmensdaten unautorisiert zu übertragen (Data Exfiltration).
- Social Engineering oder eine andere Form eines sicherheitsrelevanten Vorfalls kann nicht ausgeschlossen werden.

Die bestehende Sicherheitsblockierung darf nicht eigenständig durch den IT-Support aufgehoben oder umgangen werden.

Der Vorfall sollte dokumentiert und bei Bedarf an Information Security bzw. das zuständige Security-Team eskaliert werden.

## 3. Untersuchung

Folgende Punkte müssen überprüft werden:

- Absender und Benutzerkonto des Mitarbeiters identifizieren
- Berechtigung des Mitarbeiters zum Zugriff auf die Kundenliste überprüfen
- Fehlermeldung und Zeitpunkt der blockierten E-Mail dokumentieren
- Prüfen, ob die Blockierung durch eine DLP-Richtlinie ausgelöst wurde
- DLP-Ereignis und relevante Sicherheitsprotokolle überprüfen, sofern entsprechende Berechtigungen vorhanden sind
- Feststellen, welche Datenkategorien erkannt wurden und welche Richtlinie die Übertragung verhindert hat
- Prüfen, ob weitere verdächtige Aktivitäten oder wiederholte Übertragungsversuche vorliegen
- Bei Bedarf die Identität des Mitarbeiters über einen vertrauenswürdigen Kommunikationskanal bestätigen

## 4. Durchgeführte Maßnahmen / Geplante Maßnahmen

- Die Anfrage, Kundendaten an eine private Gmail-Adresse zu senden, wird aus Sicherheits- und Datenschutzgründen abgelehnt.
- Die bestehende DLP-Blockierung bleibt aktiv.
- Es erfolgt keine eigenständige Freischaltung oder Umgehung der Sicherheitsrichtlinie.
- Der Vorfall wird im Ticketsystem dokumentiert.
- Relevante DLP-Ereignisse und Informationen werden an Information Security bzw. das zuständige Security-Team weitergeleitet.
- Es wird geprüft, ob der Mitarbeiter über einen freigegebenen Zugriffsweg auf die Datei in SharePoint zugreifen kann.
- Dabei werden die geltenden Conditional-Access-Richtlinien und die Sicherheitsanforderungen an das verwendete Gerät berücksichtigt.
- Falls der Zugriff von privaten Geräten nicht erlaubt ist, wird eine freigegebene Alternative geprüft, beispielsweise ein Unternehmenslaptop oder eine virtuelle Arbeitsumgebung (VDI).
- Weitere Maßnahmen werden mit dem zuständigen Security-Team und gegebenenfalls der Datenschutzbeauftragten abgestimmt.

## 5. Kommunikation mit dem Benutzer

**Erste Antwort:**

Guten Tag,

vielen Dank für Ihre Nachricht.

Aus Sicherheits- und Datenschutzgründen können wir den Versand der Kundendaten an eine private E-Mail-Adresse leider nicht freischalten.

Die Datei enthält personenbezogene Informationen wie Kundenadressen und Telefonnummern. Diese Daten müssen gemäß den internen Sicherheitsrichtlinien innerhalb der dafür vorgesehenen Unternehmensumgebung verarbeitet werden.

Gerne unterstützen wir Sie dabei, eine sichere Möglichkeit für die Arbeit von zu Hause aus zu finden.

Bitte verwenden Sie dafür die von Ihrem Unternehmen freigegebenen Zugriffswege, beispielsweise den Zugriff auf die Datei über SharePoint mit Ihrem Unternehmenskonto und einem dafür zugelassenen Gerät.

Wir prüfen außerdem, ob die bestehende Blockierung durch eine DLP-Richtlinie ausgelöst wurde und ob weitere Maßnahmen erforderlich sind.

Vielen Dank für Ihr Verständnis.

Mit freundlichen Grüßen  
Ihr IT-Support

## 6. Ergebnis

Die Anfrage, die Kundendaten an eine private Gmail-Adresse zu senden, wird aus Sicherheits- und Datenschutzgründen abgelehnt.

Die bestehende DLP-Blockierung bleibt aktiv. Eine eigenständige Freischaltung oder Umgehung der Sicherheitsrichtlinie durch den IT-Support erfolgt nicht.

Der Vorfall wird dokumentiert und zur weiteren Prüfung an Information Security bzw. das zuständige Security-Team eskaliert.

Parallel wird geprüft, ob der Mitarbeiter über einen freigegebenen Zugriffsweg auf die Datei in SharePoint zugreifen kann, beispielsweise mit einem Unternehmensgerät und seinem Unternehmenskonto.

**Aktueller Status:** Die Anfrage wurde nicht freigeschaltet. Die weitere Untersuchung und die Bereitstellung eines sicheren Zugriffswegs müssen mit den zuständigen Stellen abgestimmt werden.

## 7. Eingesetzte Kenntnisse und Fähigkeiten

- Data Loss Prevention (DLP)
- Information Security
- Microsoft 365
- SharePoint
- Microsoft Entra ID
- Conditional Access
- Datenschutz und DSGVO
- Data Exfiltration Awareness
- Security Incident Recognition
- Access Management
- Least Privilege Principle
- Incident Documentation and Escalation
- User Communication

## 8. Erkenntnisse

- Data Loss Prevention (DLP) dient dazu, sensible Unternehmensdaten zu erkennen und deren unautorisierte Übertragung oder Weitergabe zu verhindern.
- Personenbezogene Daten wie Namen, Adressen und Telefonnummern müssen entsprechend den geltenden Datenschutz- und Unternehmensrichtlinien verarbeitet werden.
- Ein dringender Arbeitsauftrag oder eine nahende Abgabefrist rechtfertigt nicht die Umgehung bestehender Sicherheitsrichtlinien.
- Der IT-Support sollte bei einer DLP-Blockierung zunächst die Ursache untersuchen und die geltenden Richtlinien berücksichtigen.
- Unternehmensdaten sollten innerhalb der freigegebenen Infrastruktur verarbeitet werden, beispielsweise über SharePoint mit einem autorisierten Unternehmenskonto und einem zugelassenen Gerät.
- Conditional Access kann den Zugriff abhängig von Benutzeridentität, Gerätestatus, Standort und weiteren Sicherheitsbedingungen steuern.
- Ein VPN kann je nach Unternehmensarchitektur zusätzlich erforderlich sein, ersetzt jedoch nicht automatisch die Anforderungen von Conditional Access.
- Ein verdächtiger Datenübertragungsversuch ist nicht automatisch ein bestätigter Sicherheitsvorfall oder Phishing-Angriff.
- Der IT-Support sollte verdächtige Aktivitäten sachlich dokumentieren und bei Bedarf an Information Security eskalieren, ohne vorschnell Absicht zu unterstellen.

---

*This case study is a training simulation and does not describe a real production incident.*
