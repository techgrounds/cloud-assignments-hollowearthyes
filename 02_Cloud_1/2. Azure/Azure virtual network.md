# Azure virtual network
Aanmaken van een Virtual Network (VNet) en een virtuele machine (VM) in Microsoft Azure, met specifieke subnetconfiguraties en installatie van een Apache-webserver.

## Key-terms
- Virtual Network (VNet): Een logisch geïsoleerd netwerk in Azure waarin Azure-resources worden geplaatst en die communicatie mogelijk maakt tussen deze resources.
- Subnet: Een deel van een VNet waarin resources kunnen worden geplaatst en die een deel van het IP-adresbereik van het VNet gebruikt.
- Custom Data: Aangepaste gegevens die kunnen worden toegevoegd aan een virtuele machineconfiguratie, bijvoorbeeld scripts die worden uitgevoerd tijdens de implementatie.
- Apache Server: Een populaire open-source webserversoftware.
- SSH: Secure Shell, een protocol voor veilige netwerkcommunicatie en -besturing.
- HTTP: Hypertext Transfer Protocol, het protocol dat wordt gebruikt voor het verzenden van webpagina's over het internet.
- Public IP: Een IP-adres dat rechtstreeks bereikbaar is via het internet.

## Opdracht
1. Maak een Virtual Network (VNet) genaamd "Lab-VNet" in de West Europe-regio met de opgegeven IP-bereiken voor Subnet-1 en Subnet-2.
2. Configureer Subnet-1 zodat deze geen route naar het internet heeft.
3. Maak een virtuele machine met een Apache-webserver, waarbij de aangegeven custom data wordt gebruikt.
4. Zorg ervoor dat de virtuele machine alleen HTTP-toegang heeft en geen SSH-toegang.
5. Controleer of de website bereikbaar is vanaf het internet.

## Gebruikte bronnen
- Microsoft Azure-documentatie: https://docs.microsoft.com/azure/
- Azure Portal: https://portal.azure.com/

## Ervaren problemen
Geen problemen ondervonden bij deze opdracht.

## Resultaat
Het resultaat van deze opdracht is dat een Virtual Network is aangemaakt met de juiste subnetconfiguraties, een virtuele machine is gemaakt met een Apache-webserver en dat de website bereikbaar is vanaf het internet. Dit kan worden gecontroleerd door naar de IP-adres van de virtuele machine te navigeren in een webbrowser en te controleren of de Apache-defaultpagina wordt weergegeven. Daarnaast kan worden geverifieerd dat SSH-toegang tot de virtuele machine niet mogelijk is.