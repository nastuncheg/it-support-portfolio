# Ticket 05: Offboarding eines Mitarbeiters und Zugriff auf sein Postfach

**Ticket-Typ:** Service Request  
**Priorität:** Mittel  
**Systeme:** Microsoft 365, Exchange Online, Microsoft Entra ID  
**Status:** Training Simulation, in Bearbeitung

## 1. Problembeschreibung

Die Teamleiterin aus dem Vertrieb informiert den IT-Support, dass Herr Becker am Freitag seinen letzten Arbeitstag hat.

Sie bittet darum, seine Zugänge zu deaktivieren und ihr weiterhin Zugriff auf sein Postfach zu ermöglichen, da dort noch Kundenanfragen eingehen.

Die Teamleiterin möchte, dass alle Maßnahmen möglichst noch am selben Tag erledigt werden.

## 2. Ersteinschätzung

Es handelt sich um einen Offboarding-Service-Request mit Anforderungen an Account Management, Access Management und die Sicherstellung der Geschäftskontinuität.

Da Herr Becker erst am Freitag ausscheidet, dürfen seine Zugänge nicht ohne vorherige Abstimmung vorzeitig deaktiviert werden.

Für den weiteren Zugriff auf das Postfach bietet sich eine Umwandlung in eine Shared Mailbox in Exchange Online an. Dadurch kann die Teamleiterin mit ihrem eigenen Benutzerkonto auf die E-Mails zugreifen, ohne die Anmeldedaten von Herrn Becker verwenden zu müssen.

Zusätzlich müssen bestehende Gruppenmitgliedschaften, administrative Rollen und Eigentümerrechte überprüft werden.

## 3. Untersuchung und Vorbereitung

Folgende Punkte müssen vor der Durchführung überprüft werden:

- Offboarding-Anfrage und Genehmigung durch HR bzw. die zuständige Stelle bestätigen
- Letzten Arbeitstag und geplanten Zeitpunkt der Kontodeaktivierung abstimmen
- Benutzerkonto von Herrn Becker in Microsoft Entra ID identifizieren
- Zugehörige Microsoft 365-Gruppen und Sicherheitsgruppen überprüfen
- Administrative Rollen und besondere Berechtigungen überprüfen
- Prüfen, ob Herr Becker Eigentümer von Microsoft 365-Gruppen, Teams oder SharePoint-Sites ist
- Verantwortlichkeiten für geschäftskritische Ressourcen identifizieren und eine Übergabe vorbereiten
- Postfach in Exchange Online identifizieren
- Postfachgröße, Archivierungsfunktionen und Aufbewahrungsrichtlinien überprüfen
- Erforderliche Genehmigung für den weiteren Zugriff der Teamleiterin einholen
- Klären, ob die Teamleiterin nur E-Mails lesen und verwalten oder auch im Namen des Postfachs antworten muss

## 4. Geplante Maßnahmen

### Postfach und Berechtigungen

- Postfach von Herrn Becker nach dem vereinbarten Zeitpunkt in eine Shared Mailbox umwandeln
- Teamleiterin nach entsprechender Genehmigung Full Access erteilen
- Falls erforderlich, zusätzlich Send As vergeben
- Zugriff über Outlook bzw. Outlook Web überprüfen
- Sicherstellen, dass vorhandene E-Mails erhalten bleiben und neue Nachrichten weiterhin eingehen können

### Benutzerkonto und weitere Zugänge

- Benutzerkonto von Herrn Becker zum vereinbarten Zeitpunkt in Microsoft Entra ID deaktivieren
- Aktive Sitzungen und Refresh Tokens gemäß der internen Sicherheitsrichtlinie widerrufen
- Weitere Zugänge zu Unternehmensanwendungen und Systemen gemäß der Offboarding-Checkliste deaktivieren
- Gruppenmitgliedschaften und Berechtigungen überprüfen und gemäß der Unternehmensrichtlinie anpassen
- Eigentümerrechte und Zuständigkeiten für geschäftskritische Ressourcen nach Genehmigung übertragen

### Lizenzierung und Datenaufbewahrung

- Prüfen, ob die Exchange Online-Lizenz nach der Umwandlung weiterhin benötigt wird
- Lizenz erst entfernen, nachdem die Umwandlung und der weitere Zugriff erfolgreich überprüft wurden
- Aufbewahrungs- und Compliance-Anforderungen berücksichtigen
- Benutzerkonto nicht vorzeitig löschen, solange Aufbewahrungs- oder Wiederherstellungsanforderungen bestehen

## 5. Kommunikation mit dem Benutzer

**Erste Antwort:**

Guten Tag,

vielen Dank für Ihre Nachricht. Gerne unterstützen wir Sie beim Offboarding von Herrn Becker.

Da Herr Becker seinen letzten Arbeitstag am Freitag hat, bereiten wir die erforderlichen Maßnahmen zunächst vor und stimmen den Zeitpunkt der Deaktivierung seiner Zugänge entsprechend ab.

Für den weiteren Zugriff auf sein Postfach schlagen wir vor, dieses nach seinem Ausscheiden in eine Shared Mailbox umzuwandeln. Anschließend können wir Ihnen die erforderlichen Berechtigungen erteilen, sodass Sie weiterhin auf die vorhandenen und eingehenden E-Mails zugreifen können.

Könnten Sie uns bitte noch bestätigen, ob Sie die E-Mails lediglich lesen und verwalten müssen oder ob Sie auch im Namen des Postfachs antworten möchten?

Wir überprüfen außerdem, ob Herr Becker Eigentümer von Microsoft 365-Gruppen, Teams oder SharePoint-Sites ist und ob entsprechende Zuständigkeiten übertragen werden müssen.

Vielen Dank!

Mit freundlichen Grüßen  
Ihr IT-Support

## 6. Ergebnis

Die erforderlichen Offboarding-Maßnahmen wurden identifiziert und vorbereitet.

Das Postfach soll nach dem Ausscheiden von Herrn Becker in eine Shared Mailbox umgewandelt werden. Die Teamleiterin erhält nach entsprechender Genehmigung Full Access. Falls sie auch im Namen des Postfachs antworten muss, wird zusätzlich Send As vergeben.

Das Benutzerkonto wird zum vereinbarten Zeitpunkt deaktiviert. Bestehende Sitzungen und weitere Zugriffsrechte werden gemäß der internen Sicherheitsrichtlinie widerrufen.

Vor einer endgültigen Löschung des Benutzerkontos werden die geltenden Aufbewahrungs- und Compliance-Anforderungen berücksichtigt.

**Aktueller Status:** Die Umsetzung steht noch aus. Sie hängt von der Bestätigung des Offboardings, der Genehmigung des Postfachzugriffs und der Abstimmung des Zeitpunkts ab.

## 7. Eingesetzte Kenntnisse und Fähigkeiten

- Microsoft 365 Administration
- Exchange Online
- Microsoft Entra ID
- Shared Mailbox Management
- Berechtigungsverwaltung, Full Access und Send As
- User Account Lifecycle Management
- Offboarding-Prozesse
- Access Management und Least Privilege
- Lizenzmanagement
- Datenschutz und Datenaufbewahrung
- Dokumentation und strukturierte Fehlerbearbeitung

## 8. Erkenntnisse

- Beim Offboarding müssen sowohl Sicherheitsanforderungen als auch die Kontinuität der Geschäftsprozesse berücksichtigt werden.
- Die Weitergabe von Passwörtern oder die Nutzung fremder Anmeldedaten ist keine geeignete Lösung für den Zugriff auf ein ehemaliges Mitarbeiterpostfach.
- Eine Shared Mailbox ermöglicht berechtigten Personen den weiteren Zugriff auf E-Mails mit ihren eigenen Benutzerkonten.
- Full Access und Send As erfüllen unterschiedliche Aufgaben und sollten entsprechend dem tatsächlichen Bedarf vergeben werden.
- Vor der Deaktivierung eines Benutzerkontos müssen Gruppenmitgliedschaften, administrative Rollen und Eigentümerrechte überprüft werden.
- Die Deaktivierung und die endgültige Löschung eines Benutzerkontos sind unterschiedliche Schritte.
- Lizenzierung, Datenaufbewahrung und Compliance-Anforderungen müssen bei der Umwandlung einer Shared Mailbox berücksichtigt werden.
- Ein strukturierter Offboarding-Prozess hilft, unbefugten Zugriff zu verhindern und einen reibungslosen Übergang der Verantwortlichkeiten sicherzustellen.

---

*This case study is a training simulation and does not describe a real production incident.*
