# Phishing-Vorfall

**Szenario:** Schulungssimulation  
**Bereich:** IT-Support, Informationssicherheit  
**Rolle:** First-Level IT Support (simuliert)

## 1. Problembeschreibung

Ein Benutzer meldet eine verdächtige E-Mail. Der Absender fordert ihn auf, sein Passwort über einen enthaltenen Link zu bestätigen.

Die E-Mail weist mehrere typische Phishing-Merkmale auf:

- Unbekannte Absenderadresse
- Rechtschreibfehler im Nachrichtentext
- Aufforderung zur Eingabe von Zugangsdaten über einen Link

Der Benutzer hat den Link nicht angeklickt und keine Zugangsdaten eingegeben.

## 2. Ersteinschätzung

Es handelt sich um einen sicherheitsrelevanten Incident.

Die E-Mail weist typische Merkmale eines Phishing-Versuchs auf. Da der Benutzer den Link nicht angeklickt und keine Zugangsdaten eingegeben hat, gibt es zunächst keine konkreten Hinweise auf eine Kompromittierung seines Kontos oder Geräts.

Es muss dennoch geprüft werden, ob weitere Benutzer die Nachricht erhalten oder mit dem enthaltenen Link interagiert haben.

## 3. Untersuchung

Im Rahmen des simulierten Szenarios wurden folgende Schritte durchgeführt:

1. Analyse der verdächtigen E-Mail.
2. Überprüfung der Absenderadresse, des Nachrichteninhalts und des enthaltenen Links.
3. Identifizierung typischer Phishing-Merkmale.
4. Überprüfung der Empfänger mithilfe von Mail Flow bzw. Message Trace.
5. Prüfung, ob Benutzer mit dem enthaltenen Link interagiert haben.
6. Überprüfung auf Hinweise auf eine Kompromittierung des Benutzerkontos des meldenden Benutzers.

## 4. Durchgeführte Maßnahmen

- Die Phishing-Nachricht wurde gemäß der internen Sicherheitsrichtlinie isoliert bzw. entfernt.
- Es wurden keine Hinweise auf eine Interaktion des meldenden Benutzers mit dem Link festgestellt.
- Es wurden keine Hinweise auf eine Kompromittierung seines Benutzerkontos festgestellt.
- Falls bei anderen Benutzern eine Interaktion mit dem Link oder eine Eingabe von Zugangsdaten festgestellt würde, wäre eine Eskalation an das zuständige Security- bzw. Second-Level-Team erforderlich.

## 5. Kommunikation mit dem Benutzer

### Erste Antwort

Guten Tag,

vielen Dank, dass Sie die verdächtige E-Mail gemeldet haben und nicht auf den Link geklickt haben. Das war genau die richtige Vorgehensweise.

Wir überprüfen die E-Mail und prüfen, ob weitere Benutzer diese Nachricht erhalten haben und ob jemand mit dem enthaltenen Link interagiert hat.

Bitte klicken Sie bis dahin nicht auf den Link und antworten Sie nicht auf die Nachricht.

Mit freundlichen Grüßen  
Ihr IT-Support

### Abschlussmeldung

Guten Tag,

vielen Dank nochmals für Ihre Meldung.

Wir haben die E-Mail als Phishing-Nachricht identifiziert und entsprechende Maßnahmen eingeleitet. Für Ihr Benutzerkonto wurden keine verdächtigen Aktivitäten festgestellt.

Sie müssen aktuell keine weiteren Maßnahmen ergreifen. Bitte löschen Sie die E-Mail, falls sie sich noch in Ihrem Postfach befindet.

Vielen Dank für Ihre Aufmerksamkeit.

Mit freundlichen Grüßen  
Ihr IT-Support

## 6. Ergebnis

Die gemeldete E-Mail wurde als Phishing-Nachricht identifiziert und gemäß der internen Sicherheitsrichtlinie behandelt.

Beim meldenden Benutzer wurden keine Hinweise auf eine Interaktion mit dem Link oder eine Kompromittierung des Kontos festgestellt. Die Nachricht wurde isoliert bzw. entfernt.

## 7. Eingesetzte Kenntnisse und Fähigkeiten

- Erkennung von Phishing-Versuchen
- Analyse verdächtiger E-Mails
- Microsoft 365 Message Trace
- Incident Handling
- Informationssicherheit
- Benutzerkommunikation
- Eskalationsprozesse im IT-Support

## 8. Erkenntnisse

Auch wenn ein Benutzer nicht auf einen verdächtigen Link geklickt hat, sollte eine gemeldete Phishing-E-Mail untersucht werden.

Die Überprüfung der Empfänger und möglicher Benutzerinteraktionen hilft dabei, den Umfang eines Sicherheitsvorfalls einzuschätzen.

Der First-Level-Support sollte die internen Sicherheitsrichtlinien einhalten, verdächtige Nachrichten entsprechend behandeln und mögliche Kompromittierungen an das zuständige Security-Team eskalieren.

---

*Diese Fallstudie basiert auf einer simulierten Übung im Rahmen des Kiron Skill IT Up Programms und beschreibt keinen realen Sicherheitsvorfall.*
