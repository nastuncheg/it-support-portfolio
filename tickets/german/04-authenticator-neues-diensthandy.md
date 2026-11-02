# MFA-Problem nach Wechsel des Diensthandys

**Szenario:** Schulungssimulation  
**Bereich:** Microsoft 365, Microsoft Entra ID, Identity & Access Management  
**Priorität:** Hoch  
**Status:** Offen  
**Rolle:** First-Level IT Support (simuliert)

## 1. Problembeschreibung

Ein Benutzer hat seit dem Vortag ein neues Diensthandy und kann sich seit dem Morgen nicht mehr bei Outlook und Microsoft Teams anmelden.

Nach Eingabe des Passworts wird eine MFA-Bestätigung über Microsoft Authenticator angefordert. Die Authenticator-App auf dem neuen Diensthandy enthält jedoch keine registrierten Konten.

Der Benutzer benötigt dringend Zugriff auf Microsoft Teams, da um 10:00 Uhr ein wichtiges Kundengespräch geplant ist.

## 2. Ersteinschätzung

Die wahrscheinlichste Ursache ist, dass die bisherige MFA-Registrierung nicht auf das neue Gerät übertragen wurde.

Da der Benutzer sowohl von Outlook als auch von Teams ausgeschlossen ist und ein wichtiger Kundentermin bevorsteht, wird der Incident mit hoher Priorität behandelt.

Zunächst sollen bereits eingerichtete alternative Anmeldemethoden überprüft werden. Falls keine davon verfügbar ist, wird administrative Unterstützung benötigt.

## 3. Untersuchung und Troubleshooting

Folgende Möglichkeiten werden in der ersten Phase geprüft:

1. Verfügbarkeit von Windows Hello for Business auf dem Dienstlaptop.
2. Prüfung, ob Windows Hello for Business für die Anmeldung bei Microsoft 365 verwendet werden kann.
3. Verfügbarkeit einer zuvor registrierten SMS-Verifizierung.
4. Prüfung, ob eine alternative MFA-Methode durch die Unternehmensrichtlinien zugelassen ist.

Dabei ist zu berücksichtigen, dass Windows Hello for Business und SMS bereits eingerichtet und für den jeweiligen Anmeldevorgang zugelassen sein müssen.

## 4. Geplante Maßnahmen

Falls eine alternative Anmeldemethode verfügbar ist:

- Benutzer bei der Anmeldung über Windows Hello for Business oder SMS unterstützen.
- Prüfen, ob der Zugriff auf Outlook und Microsoft Teams wieder möglich ist.
- Anschließend die Registrierung von Microsoft Authenticator auf dem neuen Diensthandy unterstützen.

Falls keine alternative Anmeldemethode verfügbar ist:

- Fall an den Microsoft Entra ID Administrator eskalieren.
- Identität des Benutzers gemäß den internen Sicherheitsrichtlinien überprüfen lassen.
- Gegebenenfalls einen Temporary Access Pass (TAP) bereitstellen oder die MFA-Registrierung zurücksetzen lassen.
- Benutzer bei der erneuten Einrichtung von Microsoft Authenticator unterstützen.

## 5. Kommunikation mit dem Benutzer

### Erste Antwort

Guten Morgen,

vielen Dank für Ihre Nachricht. Ich verstehe, dass die Situation vor Ihrem wichtigen Kundengespräch stressig ist. Wir kümmern uns schnellstmöglich darum.

Bitte versuchen Sie zunächst folgende alternative Anmeldemethoden:

**1. Windows Hello for Business**

Falls Windows Hello for Business auf Ihrem Dienstlaptop bereits eingerichtet ist, versuchen Sie bitte, sich damit bei Microsoft 365 anzumelden. Wählen Sie dazu gegebenenfalls „Anmeldeoptionen“ aus.

**2. SMS-Verifizierung**

Falls Sie SMS als alternative MFA-Methode registriert haben und diese von Ihrer Organisation zugelassen ist, können Sie versuchen, den Anmeldecode per SMS zu erhalten.

Falls keine dieser Möglichkeiten funktioniert, geben Sie uns bitte kurz Bescheid. Wir prüfen dann die nächsten Schritte.

Gegebenenfalls muss unser IT-Administrator Ihre Identität überprüfen und Ihnen einen Temporary Access Pass (TAP) bereitstellen oder die MFA-Registrierung zurücksetzen, damit Sie Microsoft Authenticator auf Ihrem neuen Diensthandy erneut einrichten können.

Vielen Dank für Ihre Geduld.

Viele Grüße  
Ihr IT-Support

## 6. Aktueller Status

**Status:** Offen

Es liegt noch keine Rückmeldung des Benutzers zu den vorgeschlagenen alternativen Anmeldemethoden vor.

Die tatsächliche Ursache und die erfolgreiche Wiederherstellung des Zugriffs müssen noch bestätigt werden.

## 7. Eingesetzte Kenntnisse und Fähigkeiten

- Microsoft 365 Support
- Microsoft Authenticator
- Multi-Factor Authentication (MFA)
- Microsoft Entra ID
- Windows Hello for Business
- Temporary Access Pass (TAP)
- Identity & Access Management
- Incident Priorisierung
- Eskalationsmanagement
- Benutzerkommunikation

## 8. Erkenntnisse

Beim Wechsel eines Diensthandys müssen die registrierten MFA-Methoden auf dem neuen Gerät erneut eingerichtet werden, sofern sie nicht erfolgreich übertragen werden können.

Alternative Anmeldemethoden wie Windows Hello for Business oder SMS können helfen, den Zugriff wiederherzustellen, sofern sie bereits eingerichtet und durch die Unternehmensrichtlinien zugelassen sind.

Wenn keine alternative Authentifizierungsmethode verfügbar ist, kann ein Administrator nach erfolgreicher Identitätsprüfung einen Temporary Access Pass bereitstellen oder die MFA-Registrierung zurücksetzen.

Ein wichtiger Grundsatz im IT-Support ist, die Arbeitsfähigkeit des Benutzers schnell wiederherzustellen, ohne dabei die Sicherheitsrichtlinien zu umgehen.

---

*Diese Fallstudie basiert auf einer simulierten Übung im Rahmen des IT-Support-Trainings und beschreibt keinen realen Supportvorfall.*
