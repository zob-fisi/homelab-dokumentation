# Übung 02: VNet und Subnetze in Azure

**Datum:** 09.11.2026
**Ziel:** Ein virtuelles Netzwerk (VNet) mit zwei Subnetzen im Azure-Portal anlegen und verstehen, wie es aufgebaut ist.

## Was ich gemacht habe
1. VNet `vnet-test01` in der Ressourcengruppe `rg-homelab-lab` erstellt
2. Region: `Germany-West-Central`
3. Address space: `10.0.0.0/16`
4. Subnetz `default`: `10.0.0.0/24`
5. Zweites Subnetz `subnet-test02: 10.0.1.0/24` 
6. Optionen unter "Security" (Bastion, Firewall, DDoS) bewusst deaktiviert, weil sie zusätzliche Kosten verursachen können.

## Screenshots
![VNet Übersicht](screenshots/vnet-uebersicht.png)
![Subnetze](screenshots/subnetze.png)

*(Subscription-ID und andere Kennungen sind geschwärzt.)*

## Was ich gelernt habe
- Ein VNet ist ein privates Netzwerk in Azure, das in Subnetze unterteilt wird.
- Der Address space des VNet legt fest, aus welchem Bereich die Subnetze stammen.
- Ein /24-Subnetz hat 256 Adressen, angezeigt werden aber nur 251. Soweit ich weiß, reserviert Azure pro Subnetz 5 Adressen für sich.

## Probleme
- Beim Versuch, eine VM zu erstellen, kam in allen Regionen die Meldung `NotAvailableForSubscription`. Ich habe deshalb zuerst das VNet geübt. Die VM hole ich später nach.

## Aufräumen
- VNet nach der Übung gelöscht, Ressourcengruppe wieder leer.
