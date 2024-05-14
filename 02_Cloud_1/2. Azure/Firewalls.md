# Firewalls
Implementatie van Network Security Group (NSG) in Azure om SSH-verkeer te blokkeren en HTTP-verkeer toe te staan.

## Key-terms
- Azure: Microsoft's cloud computing platform offering a variety of services.
- Network Security Group (NSG): A security group containing a list of security rules that allow or deny network traffic to resources in an Azure virtual network.
- SSH: Secure Shell, a cryptographic network protocol used for secure communication over an unsecured network.
- HTTP: Hypertext Transfer Protocol, the foundation of data communication for the World Wide Web.
- Virtual Network (VNET): A logically isolated network in the Azure cloud where Azure resources are deployed.
- Webserver: A server software or hardware dedicated to running services over the World Wide Web.
- Inbound rule: A rule in a NSG that controls incoming traffic to Azure resources.
- Outbound rule: A rule in a NSG that controls outgoing traffic from Azure resources.

## Opdracht
1. Start een webserver en zorg ervoor dat poorten voor zowel SSH als HTTP geopend zijn.
2. Maak een NSG in het VNET om SSH-verkeer te blokkeren en HTTP-verkeer toe te staan.
3. Test of de NSG correct werkt door te proberen SSH-toegang te verkrijgen en de webserver te bereiken via HTTP.

## Gebruikte bronnen
- Microsoft Azure-documentatie: https://docs.microsoft.com/azure/
- Azure Portal: https://portal.azure.com/

## Ervaren problemen
Geen problemen ondervonden bij deze opdracht.

## Resultaat
De opdracht is geslaagd als SSH-toegang tot de webserver wordt geblokkeerd en de webserver nog steeds bereikbaar is via HTTP. Dit kan worden geverifieerd door te proberen SSH-toegang te verkrijgen (wat zou moeten falen) en door de webserver te openen in een webbrowser. Als de webpagina van de webserver wordt weergegeven, is de opdracht gelukt.

Als je de NSG-regels wilt instellen, kun je dit doen via de Azure Portal. Ga naar de NSG die je hebt gemaakt, voeg een inbound rule toe om poort 80 (HTTP) toe te staan en voeg een andere inbound rule toe om poort 22 (SSH) te blokkeren.