# Homelab-Dokumentation

Hier dokumentiere ich meine praktischen Übungen in **Azure** und **Linux**. Ich mache eine Umschulung zum **Fachinformatiker für Systemintegration (IHK)** (Abschluss August 2028).

**Ziel:** Cloud-Administration mit Azure lernen und mich danach in Richtung **Cloud Security** spezialisieren. Dieses Repository ist mein Lerntagebuch und mein Nachweis, dass ich das Gelernte praktisch anwenden kann.

> Stand: Oktober 2026 · Das Repository wächst mit meinem Lernfortschritt.

## Lernpfad

| Nr. | Übung | Thema | Status |
|---|---|---|---|
| 01 | Azure-Konto und Kostenkontrolle | Konto anlegen, Budget-Warnung einrichten, Ressourcengruppe mit Tags | in Arbeit |
| 02 | Erste virtuelle Maschine | VM erstellen, per SSH/RDP verbinden, wieder löschen | erledigt |
| 03 | Virtuelles Netzwerk | VNet, Subnetze, Netzwerksicherheitsgruppen (NSG) | geplant |
| 04 | Storage und Zugriffsrechte | Storage-Account, Redundanz, Rollen (RBAC) | geplant |
| 05 | Identität | Microsoft Entra ID, Benutzer und Gruppen, MFA | geplant |
| 06 | Automatisierung | Azure CLI und Bash-Skripte | geplant |
| 07 | Infrastructure as Code | Erste Umgebung mit Terraform | geplant |
| 08 | Monitoring und Sicherheit | Azure Monitor, Grundlagen Defender for Cloud | geplant |

## Zertifizierungen (Ziele)

- **AZ-900** Microsoft Azure Fundamentals: optional, geplant Dezember 2026
- **AZ-104** Microsoft Azure Administrator: geplant Juni 2027 (alternativ Herbst 2027)

## Aufbau des Repositories

```text
homelab-dokumentation/
├── README.md
├── 01-azure-konto/
│   └── README.md
├── 02-erste-vm/
│   └── README.md
├── 03-virtuelles-netzwerk/
│   └── README.md
└── ...
```

Jede Übung hat einen eigenen Ordner mit einer `README.md` nach der folgenden Vorlage.

## Vorlage pro Übung

```markdown
# Übung XX: Titel

## Ziel
Was wollte ich lernen oder bauen?

## Umgebung
Verwendete Dienste und Werkzeuge (zum Beispiel Azure, Cloud Shell, Linux).

## Schritte
1. ...
2. ...

## Ergebnis
Was funktioniert jetzt? (Screenshot, IDs und Namen unkenntlich gemacht)

## Probleme und Lösungen
Siehe Incident-Vorlage unten.

## Kosten
Ungefähre Kosten und ob alle Ressourcen danach gelöscht wurden.

## Gelernt
Zwei bis drei Sätze, was ich mitnehme.
```

## Vorlage für Probleme (Incident)

| Feld | Inhalt |
|---|---|
| Beschreibung | Was ist passiert? |
| Auswirkung | Was ging dadurch nicht? |
| Ursache | Warum ist es passiert? |
| Lösung | Wie habe ich es behoben? |
| Maßnahmen | Was mache ich künftig anders? |

## Sicherheit und Datenschutz

Umschüler zum Fachinformatiker für Systemintegration in der Region Trier, mit Interesse an Cloud und Cloud Security.


