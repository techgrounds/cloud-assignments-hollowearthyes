# Firewalls

## Onderwerp
In dit markdown-bestand behandelen we verschillende aspecten van netwerkbeveiliging, met de nadruk op firewalls en het installeren van een webserver op een Ubuntu-server. We zullen de verschillende soorten firewalls, het installatieproces van een populaire webserver (Apache) en het configureren van firewallregels met UFW bespreken.

## Key-terms
- Firewall: Een beveiligingsmechanisme dat verkeer tussen een netwerk en externe netwerken regelt, waarbij ongewenst verkeer wordt geblokkeerd en toegestaan verkeer wordt doorgelaten.
- UFW (Uncomplicated Firewall): Een frontend voor iptables, een tool voor het configureren van firewallregels in Linux-systemen.
- Apache HTTP Server: Een populaire webserversoftware die veel wordt gebruikt voor het hosten van websites en webtoepassingen.
- Firewall: Een beveiligingsmechanisme dat verkeer tussen een netwerk en externe netwerken regelt, waarbij ongewenst verkeer wordt geblokkeerd en toegestaan verkeer wordt doorgelaten.
- Stateful Firewall: Een firewall die de staat van actieve verbindingen bewaakt en beslissingen neemt op basis van de context van het verkeer. Deze firewall houdt een staatstabel bij om de staat van netwerkverbindingen te volgen.
- Stateless Firewall: Een firewall die pakketten filtert op basis van statische criteria zoals bron- en bestemmings-IP-adressen, poortnummers en protocoltypen, zonder de staat van verbindingen bij te houden.
- Hardware Firewall: Een fysiek apparaat dat is ontworpen voor het filteren van netwerkverkeer. Deze firewalls worden vaak ingezet aan de rand van een netwerk, zoals tussen het interne netwerk en het internet.
- Software Firewall: Een softwaretoepassing die op individuele computers of servers wordt geïnstalleerd om inkomend en uitgaand netwerkverkeer te controleren.

## Opdracht
1. Het begrijpen van verschillende soorten firewalls, inclusief stateful en stateless firewalls, en hardware- en software-implementaties.
2. Het installeren van Apache HTTP Server op een Ubuntu-server en het controleren van de installatie.
3. Het configureren van UFW (Uncomplicated Firewall) om alleen SSH-verkeer toe te staan en al het andere verkeer te blokkeren.

## Gebruikte bronnen
- Ubuntu Documentation: [UFW - Uncomplicated Firewall](https://help.ubuntu.com/community/UFW)
- DigitalOcean Community Tutorials: [How To Set Up a Firewall with UFW on Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu-18-04)

## Ervaren problemen
Tijdens de uitvoering van de opdracht kunnen verschillende problemen optreden:
- Het onjuist configureren van firewallregels kan leiden tot onbedoeld blokkeren van legitiem verkeer, zoals SSH-toegang.
- Fouten tijdens het installatieproces van Apache of het starten van de Apache-service kunnen problemen veroorzaken bij het hosten van websites.
- Onverwachte configuratieproblemen met UFW kunnen resulteren in ontoegankelijkheid van de server via het netwerk.

## Resultaat
Na het voltooien van de opdracht kunnen we ervan uitgaan dat:
- We in staat zijn geweest om Apache HTTP Server succesvol te installeren op onze Ubuntu-server door de juiste stappen te volgen.
- UFW correct is geconfigureerd om alleen SSH-verkeer toe te staan en al het andere verkeer te blokkeren.
- De firewall werkt zoals bedoeld door het uitvoeren van tests om inkomend en uitgaand internetverkeer te controleren en te verifiëren of de verwachte resultaten worden behaald.

![start apache](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/cf8b872b9012913b37022f273f1f568a56c704d2/00_includes/Security1/Firewalls/apache%20start.png)

Hier zijn de gebruikte commando's voor het instellen van UFW en het blokkeren van webverkeer:

![deny port 80](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/cf8b872b9012913b37022f273f1f568a56c704d2/00_includes/Security1/Firewalls/deny%20port%2080.png)

```bash
# Blokkeer al het inkomende en uitgaande webverkeer
sudo ufw deny out 80/tcp
sudo ufw deny out 443/tcp
sudo ufw deny in 80/tcp
sudo ufw deny in 443/tcp

# Sta inkomend SSH-verkeer toe (pas de poort aan indien nodig)
sudo ufw allow ssh

# Schakel de firewall in
sudo ufw enable
```
### Allowing ssh

```bash
# Sta inkomend SSH-verkeer toe (pas de poort aan indien nodig)
sudo ufw allow ssh

# Schakel de firewall in
sudo ufw enable
```

![allow ssh](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/cf8b872b9012913b37022f273f1f568a56c704d2/00_includes/Security1/Firewalls/allow%20ssh.png)
