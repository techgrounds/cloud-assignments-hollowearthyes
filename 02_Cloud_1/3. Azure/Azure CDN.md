# Azure CDN Educational Guide

## Wat is Azure CDN?

Azure Content Delivery Network (CDN) is een wereldwijd gedistribueerd netwerk van servers dat statische inhoud, zoals afbeeldingen, video's, JavaScript-bestanden en andere webinhoud, levert aan gebruikers met een hoge snelheid en lage latentie. Het optimaliseert de levering van webinhoud door de afstand tussen de gebruiker en de inhoud te verminderen, waardoor de laadtijd van webpagina's wordt verbeterd en de algehele gebruikerservaring wordt verhoogd.

### Probleemoplossing

Azure CDN lost het probleem op van trage laadtijden van webinhoud voor gebruikers over de hele wereld door statische inhoud dichter bij hen te brengen met behulp van een wereldwijd netwerk van edge-locaties. Hierdoor kunnen websites en applicaties snel en efficiënt worden geladen, zelfs voor gebruikers op afgelegen locaties.

### Belangrijke termen

- **Edge-locaties**: Servers die zich bevinden op strategische locaties over de hele wereld en die dienen als caches voor statische inhoud om snelle levering aan eindgebruikers mogelijk te maken.
- **Pull-versus-push CDN**: Pull-CDN's halen inhoud op van de oorspronkelijke server wanneer deze voor het eerst wordt aangevraagd en slaan deze vervolgens op in de cache op de edge-locaties. Push-CDN's vereisen dat inhoud handmatig wordt geüpload naar edge-locaties voordat deze wordt aangevraagd.
- **POP (Point of Presence)**: Een fysieke locatie waar CDN-infrastructuur aanwezig is om inhoud te cachen en te leveren aan gebruikers in de buurt.

### Integratie met on-premises omgevingen

Azure CDN kan worden geïntegreerd in on-premises omgevingen door middel van:

- **Aangepaste herkomsten**: Hiermee kunnen on-premises servers worden geconfigureerd als oorsprongservers voor de CDN, zodat ze statische inhoud kunnen leveren aan de edge-locaties.
- **Hybride netwerkverbindingen**: Door gebruik te maken van Azure ExpressRoute of VPN-gateways, kunnen on-premises systemen communiceren met Azure CDN voor het beheer en de configuratie van de dienst.

### Combinatie met andere diensten

Azure CDN kan worden gecombineerd met verschillende andere Azure-diensten, zoals:

- **Azure Blob Storage**: Voor het hosten van statische inhoud, zoals afbeeldingen en video's, die vervolgens wordt geleverd via Azure CDN voor snelle levering aan eindgebruikers.
- **Azure App Service**: Voor het hosten van dynamische webinhoud die kan worden gecombineerd met statische inhoud die wordt geleverd via Azure CDN voor een verbeterde gebruikerservaring.
- **Azure Front Door**: Voor het maken van geavanceerde routingregels en het optimaliseren van de levering van zowel statische als dynamische inhoud via Azure CDN.

### Verschillen met andere gelijkaardige diensten

In vergelijking met het hosten van statische inhoud op traditionele webinfrastructuur of het gebruik van andere CDN-diensten biedt Azure CDN:

- **Wereldwijd gedistribueerd netwerk**: Azure CDN maakt gebruik van een wereldwijd netwerk van edge-locaties, waardoor de levering van inhoud aan eindgebruikers over de hele wereld wordt geoptimaliseerd.
- **Integratie met Azure-services**: Azure CDN kan naadloos worden geïntegreerd met andere Azure-services, waardoor ontwikkelaars een geïntegreerde oplossing krijgen voor het hosten en leveren van webinhoud.
- **Diepe integratie met Azure Portal**: Azure CDN kan worden beheerd en geconfigureerd via de Azure Portal, waardoor het eenvoudig is om de dienst te implementeren en te beheren binnen de Azure-omgeving.

### Praktische takenlijst

1. **Dienst vinden in de console**: Navigeer naar de Azure Portal en zoek naar "Content Delivery Network" in de dienstencatalogus.
2. **Dienst inschakelen**: Klik op "Maken" om een nieuwe Azure CDN-profiel en endpoint te maken en volg de instructies om de configuratie te voltooien.
3. **Dienst koppelen aan andere resources**: Gebruik de opties voor integratie in de Azure Portal om Azure CDN te koppelen aan andere Azure-resources, zoals Blob Storage-accounts of App Services.

Dit educatieve markdown-bestand biedt een overzicht van Azure CDN, inclusief de problemen die het oplost, belangrijke termen, integratie met on-premises omgevingen, combinatiemogelijkheden met andere diensten, verschillen met vergelijkbare diensten en een praktische takenlijst voor het gebruik ervan.