# VMSS
Het implementeren van een Virtual Machine Scale Set (VMSS) met Autoscaling en het testen van de load balancing functionaliteit in Microsoft Azure.

## Key-terms
- Virtual Machine Scale Set (VMSS): Een beheerde schaalset van identieke virtuele machines die worden uitgevoerd in Azure.
- Autoscaling: Een functie die automatisch het aantal virtuele machines in een VMSS aanpast op basis van gedefinieerde schalingsregels.
- Load Balancer: Een dienst die het verkeer verdeelt over meerdere servers om de belasting te verdelen en de beschikbaarheid van de applicatie te verbeteren.
- Azure Load Balancer (ALB): Een load balancer service op laag 4 van de OSI-stack die wordt gebruikt om het verkeer te routeren naar virtuele machines in Azure.
- Application Gateway: Een load balancer service op laag 7 van de OSI-stack die geavanceerde mogelijkheden biedt zoals SSL-terminatie en Web Application Firewall (WAF) functies.
- Custom Data: Aangepaste gegevens die worden gebruikt tijdens het implementeren van een virtuele machine, zoals installatiescripts.
- Scaling Policy: Regels die bepalen wanneer en hoeveel virtuele machines er worden toegevoegd of verwijderd uit een VMSS op basis van bepaalde criteria, zoals CPU-gebruik.

## Opdracht
1. Maak een Virtual Machine Scale Set met de opgegeven vereisten, inclusief Autoscaling policy.
2. Controleer of de webserver bereikbaar is via het endpoint van de load balancer.
3. Voer een load test uit om Autoscaling te activeren en controleer of nieuwe virtuele machines worden gemaakt volgens de schalingsregels.

## Gebruikte bronnen
- Microsoft Azure-documentatie: https://docs.microsoft.com/azure/
- Azure Portal: https://portal.azure.com/

## Ervaren problemen
Geen problemen ondervonden bij deze opdracht.

## Resultaat
Het resultaat van deze opdracht is dat een Virtual Machine Scale Set is aangemaakt met de juiste configuratie en dat de webserver bereikbaar is via het endpoint van de load balancer. Door een load test uit te voeren, kan worden gecontroleerd of Autoscaling correct wordt geactiveerd en of nieuwe virtuele machines worden toegevoegd volgens de schalingsregels. Screenshots kunnen worden gebruikt om de configuratie en het resultaat van de opdracht te documenteren.