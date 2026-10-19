[README.md](https://github.com/user-attachments/files/33665253/README.md)
# Übung 01: Azure-Konto, Kostenkontrolle und Ressourcengruppe

## Ziel

Ein eigenes Azure-Gratiskonto anlegen, es absichern und so einrichten, dass keine ungewollten Kosten entstehen. Dazu lege ich eine erste Ressourcengruppe mit Tags an, in der alle späteren Übungen laufen.

## Umgebung

- Azure Free Account (200 $ Startguthaben für 30 Tage)
- Azure-Portal im Browser
- Anmeldung mit persönlichem Konto, nicht mit einem Konto der Bildungseinrichtung

## Schritte

- [x] Gratiskonto auf azure.microsoft.com/free angelegt (19.10.2026)
- [x] Zwei-Faktor-Anmeldung (MFA) für das Konto aktiviert
- [x] Budget mit E-Mail-Warnungen bei 50 %, 80 % und 100 % eingerichtet (Cost Management, Budgets)
- [x] Ressourcengruppe `rg-homelab-lab` in einer europäischen Region erstellt
- [x] Tags gesetzt: `umgebung = lab`, `zweck = lernen`
- [ ] Cost Analysis geprüft (Anzeige: 0 €)

## Ergebnis

*[Screenshot hier einfügen: Budget mit Warnstufen]*

*[Screenshot hier einfügen: Ressourcengruppe mit Tags]*

Vor dem Hochladen unkenntlich machen: Subscription-ID, E-Mail-Adresse, Kartendaten und Tenant-ID.

## Probleme und Lösungen

### Incident 1: Anmeldung am Azure-Portal schlägt fehl

| Feld | Inhalt |
|---|---|
| Beschreibung | Beim Öffnen des Azure-Portals erschien der Fehler AADSTS90072. Die Anmeldung wurde abgelehnt. |
| Auswirkung | Kein Zugriff auf das Portal, die Einrichtung des Gratiskontos war blockiert. |
| Ursache | Die Anmeldung lief über den Mandanten (Tenant) der Bildungseinrichtung. Mein persönliches Microsoft-Konto war dort nicht als externer Benutzer eingetragen. Wahrscheinlich war noch eine Sitzung der Bildungseinrichtung im Browser aktiv. |
| Lösung | Privates Browserfenster geöffnet und das Gratiskonto direkt über die offizielle Free-Account-Seite angelegt. Dabei entstand ein eigener Tenant. |
| Maßnahmen | Für private Übungen immer ein privates Browserfenster oder ein eigenes Browserprofil nutzen. Bei einem Verzeichniswechsel im Portal oben rechts auf das Profilbild gehen und das richtige Verzeichnis wählen. |

## Kosten

- Startguthaben: 200 $, nutzbar in den ersten 30 Tagen ab Anmeldung
- Budget-Warnung: 5$ und 8$
- Bisherige Kosten: 0$ 
- Alle Übungsressourcen werden nach der Übung gelöscht: ja

## Gelernt

- Ein **Tenant** ist ein eigenes Verzeichnis mit eigenen Benutzern. Ein Konto kann in mehreren Tenants vorkommen, aber nicht automatisch überall zugreifen.
- Ein **Budget** warnt nur, es stoppt keine Ressourcen. Kostenkontrolle heißt deshalb: Budget setzen und selbst aufräumen.
- Eine **Ressourcengruppe** bündelt Ressourcen. Löscht man die Gruppe, werden alle Ressourcen darin gelöscht.


