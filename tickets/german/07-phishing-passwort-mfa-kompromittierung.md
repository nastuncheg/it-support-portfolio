# Passwort auf einer Phishing-Seite eingegeben, möglicher Account Compromise

**Incident-Typ:** Security Incident  
**Priorität:** Hoch  
**Systeme:** Microsoft 365, Microsoft Entra ID, Microsoft Authenticator, Exchange Online  
**Status:** Training Simulation, an Information Security eskaliert

## 1. Problembeschreibung

Ein Benutzer erhält eine E-Mail, die angeblich von Microsoft stammt und ihn darüber informiert, dass sein Postfach voll sei.

Der Benutzer klickt auf den enthaltenen Link und gibt auf der geöffneten Seite sein Unternehmenspasswort ein. Anschließend wird lediglich eine leere Seite angezeigt.

Zusätzlich berichtet der Benutzer, dass er möglicherweise eine Anmeldeanfrage auf seinem Mobiltelefon über Microsoft Authenticator bestätigt hat.

Der Benutzer meldet den Vorfall etwa 20 Minuten nach der Interaktion mit der verdächtigen E-Mail beim IT-Support.

## 2. Ersteinschätzung

Es handelt sich um einen sicherheitskritischen Incident mit einem konkreten Verdacht auf eine Kompromittierung des Benutzerkontos (Account Compromise).

Da der Benutzer sowohl sein Passwort eingegeben als auch möglicherweise eine MFA-Anfrage bestätigt hat, besteht das Risiko, dass ein Angreifer bereits Zugriff auf das Microsoft-365-Konto erhalten hat.

Die unmittelbare Priorität liegt auf der Eindämmung der möglichen Kompromittierung (Containment).

Der Vorfall muss mit hoher Priorität an Information Security bzw. das zuständige Security Operations Team eskaliert werden.

## 3. Untersuchung

Folgende Punkte müssen überprüft werden:

- Identität des Benutzers gemäß der unternehmensinternen Sicherheitsrichtlinie bestätigen
- Zeitpunkt der Phishing-Interaktion dokumentieren
- Sign-in Logs in Microsoft Entra ID überprüfen
- Erfolgreiche und fehlgeschlagene Anmeldeversuche untersuchen
- Unbekannte IP-Adressen und ungewöhnliche geografische Standorte identifizieren
- Unbekannte Geräte und Anwendungen überprüfen
- Authentication Details und MFA-Ergebnisse untersuchen
- Ergebnisse der Conditional-Access-Prüfungen berücksichtigen
- Prüfen, ob nach der Phishing-Interaktion erfolgreiche Anmeldungen von unbekannten Standorten oder Geräten stattgefunden haben
- Postfach auf verdächtige Inbox Rules, automatische Weiterleitungen und unbekannte Delegierungen überprüfen
- Prüfen, ob verdächtige OAuth-Anwendungen autorisiert wurden oder unbekannte Berechtigungen vorliegen
- Möglichen Zugriff auf weitere Microsoft-365-Ressourcen wie Outlook, Teams, SharePoint und OneDrive untersuchen
- Prüfen, ob weitere Benutzer die gleiche Phishing-Nachricht erhalten haben

## 4. Durchgeführte Maßnahmen / Geplante Maßnahmen

### Sofortmaßnahmen, Containment

- Vorfall mit hoher Priorität dokumentieren und unverzüglich an Information Security bzw. das Security Operations Team eskalieren
- Anfordern, dass das Benutzerkonto in Microsoft Entra ID für weitere Anmeldungen gesperrt wird (Block sign-in)
- Bestehende aktive Sitzungen und Refresh Tokens widerrufen (Revoke sessions)
- Sichere Passwortänderung über einen offiziellen Unternehmenskanal veranlassen
- MFA-Methoden des Benutzers überprüfen
- Bei Bedarf bestehende MFA-Registrierungen zurücksetzen und eine erneute Registrierung über einen sicheren Prozess veranlassen

### Weitere Untersuchung

- Sign-in Logs auf nicht autorisierte Anmeldungen überprüfen
- Verdächtige Postfachregeln und automatische Weiterleitungen untersuchen
- OAuth-Berechtigungen und verbundene Anwendungen überprüfen
- Möglichen Zugriff auf weitere Unternehmensressourcen untersuchen
- Verdächtige E-Mail einschließlich Absender, Inhalt und enthaltenem Link für die weitere Analyse sichern
- Prüfen, ob weitere Benutzer betroffen sind
- Alle Untersuchungsergebnisse und durchgeführten Maßnahmen im Ticketsystem dokumentieren

## 5. Kommunikation mit dem Benutzer

**Erste Antwort:**

Guten Tag,

vielen Dank, dass Sie uns sofort informiert haben. Bitte machen Sie sich keine Vorwürfe, solche Phishing-Nachrichten können sehr überzeugend aussehen.

Da Sie Ihr Passwort eingegeben und möglicherweise auch eine MFA-Anfrage bestätigt haben, besteht der Verdacht, dass Ihr Microsoft-365-Konto kompromittiert wurde.

Wir behandeln den Vorfall mit hoher Priorität und leiten umgehend die erforderlichen Sicherheitsmaßnahmen ein.

Bitte beachten Sie bis auf Weiteres folgende Hinweise:

- Klicken Sie nicht erneut auf den Link in der E-Mail.
- Bestätigen Sie keine weiteren Anmeldeanfragen in der Authenticator-App, die Sie nicht selbst ausgelöst haben.
- Versuchen Sie nicht, sich über den Link aus der E-Mail erneut anzumelden.
- Informieren Sie uns bitte, ob Sie nach der Bestätigung der MFA-Anfrage weitere ungewöhnliche Aktivitäten bemerkt haben.

Wir melden uns schnellstmöglich mit den nächsten Schritten bei Ihnen.

Vielen Dank für Ihre schnelle Reaktion.

Mit freundlichen Grüßen  
Ihr IT-Support

## 6. Ergebnis

Der Vorfall wird als möglicher Account Compromise mit hoher Priorität behandelt und an Information Security bzw. das Security Operations Team eskaliert.

Als erste Sicherheitsmaßnahmen werden die Blockierung weiterer Anmeldungen und der Widerruf bestehender Sitzungen veranlasst. Anschließend wird eine sichere Passwortänderung durchgeführt und die MFA-Registrierung überprüft.

Die Sign-in Logs in Microsoft Entra ID werden untersucht, um festzustellen, ob ein unbefugter Zugriff stattgefunden hat.

Besondere Aufmerksamkeit gilt erfolgreichen Anmeldungen von unbekannten IP-Adressen, Standorten oder Geräten nach der Phishing-Interaktion.

Zusätzlich werden mögliche Änderungen an den Postfacheinstellungen, verdächtige Inbox Rules und OAuth-Berechtigungen überprüft.

**Aktueller Status:** An Information Security eskaliert. Die weitere Untersuchung und die Wiederherstellung des Benutzerkontos erfolgen in Abstimmung mit dem zuständigen Security-Team.

## 7. Eingesetzte Kenntnisse und Fähigkeiten

- Microsoft Entra ID
- Microsoft Authenticator
- Multi-Factor Authentication (MFA)
- Sign-in Logs und Authentication Details
- Conditional Access
- Account Compromise Recognition
- Incident Response und Containment
- Exchange Online
- Inbox Rules und Mailbox Security
- OAuth Permissions
- Security Incident Documentation
- Incident Escalation
- User Communication und Security Awareness

## 8. Erkenntnisse

- Wenn ein Benutzer seine Zugangsdaten auf einer Phishing-Seite eingegeben hat, muss von einer möglichen Kompromittierung des Benutzerkontos ausgegangen werden.
- Besonders kritisch ist es, wenn zusätzlich eine MFA-Anfrage bestätigt wurde.
- In einem solchen Fall hat die Eindämmung des Sicherheitsvorfalls (Containment) höchste Priorität.
- Eine reine Passwortänderung reicht nicht immer aus, da bereits bestehende Sitzungen weiterhin gültig sein können.
- Microsoft Entra ID bietet mit den Sign-in Logs die Möglichkeit, Anmeldeaktivitäten genauer zu untersuchen.
- Dabei sollten insbesondere IP-Adressen, geografische Standorte, verwendete Geräte, Anwendungen und MFA-Ergebnisse berücksichtigt werden.
- Ein erfolgreicher Anmeldeversuch von einer unbekannten IP-Adresse oder einem ungewöhnlichen Standort kann auf einen unbefugten Zugriff hindeuten.
- Die Untersuchung sollte nicht nur das Benutzerkonto selbst, sondern auch verbundene Microsoft-365-Dienste umfassen. Dazu gehören Outlook, Teams, SharePoint und OneDrive.
- Besonders wichtig ist die Überprüfung verdächtiger Postfachregeln, automatischer Weiterleitungen und OAuth-Berechtigungen.
- Der IT-Support sollte seine eigenen Berechtigungsgrenzen kennen. Wenn First-Level Support keine administrativen Rechte zur Kontosperrung oder zum Widerruf von Sitzungen besitzt, müssen diese Maßnahmen unverzüglich an das zuständige Team weitergegeben werden.
- Eine schnelle Meldung durch den Benutzer kann entscheidend dazu beitragen, den möglichen Schaden zu begrenzen. Deshalb sollte eine solche Meldung sachlich und unterstützend behandelt werden, ohne dem Benutzer Vorwürfe zu machen.

---

*This case study is a training simulation and does not describe a real production incident.*
