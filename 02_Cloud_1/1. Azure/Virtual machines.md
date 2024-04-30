# Virtual machines
Het maken en beheren van Azure Virtual Machines (VMs) in Microsoft Azure.

## Key-terms
- **Azure Virtual Machines**: De service in Azure waarmee je virtuele machines kunt maken en beheren.
- **Image**: Een blauwdruk voor de VM, inclusief het besturingssysteem.
- **VM Sizes**: Verschillende configuraties van VMs met verschillende hoeveelheden resources.
- **OS Disk**: De hoofdschijf van de VM waarop het besturingssysteem wordt geïnstalleerd.
- **Data Disks**: Optionele extra schijven voor gegevensopslag.
- **NIC Network Security Group**: Een beveiligingsgroep op netwerkinterface-niveau voor het beveiligen van het verkeer naar en van de VM.
- **Custom Data**: Gegevens die tijdens het opstarten aan de VM worden doorgegeven, zoals cloud-init scripts of configuratiebestanden.
- **User Data**: Een verbeterde versie van Custom Data die gedurende de hele levensduur van de VM beschikbaar blijft.

## Opdracht
1. Ga naar de Azure-portal (https://portal.azure.com/).
2. Klik op "Virtual Machines" in het zijmenu om een nieuwe VM te maken.
3. Kies een naam voor de VM en selecteer een regio waarin de VM wordt gehost.
4. Selecteer een image voor het besturingssysteem van de VM, zoals Windows Server of Ubuntu Linux.
5. Kies een VM-size op basis van de benodigde resources, zoals vCPUs, RAM en opslag.
6. Configureer de OS Disk en eventuele extra Data Disks, inclusief het type (Premium SSD, Standard SSD, Standard HDD).
7. Voeg optioneel een NIC Network Security Group toe voor beveiliging.
8. Voeg Custom Data toe als je automatische configuratie tijdens het opstarten wilt uitvoeren.
9. Controleer de prijs van de VM op basis van de geselecteerde opties.
10. Klik op "Maken" om de VM te implementeren.

## Gebruikte bronnen
- Azure-documentatie: https://docs.microsoft.com/en-us/azure/virtual-machines/

## Ervaren problemen
Een mogelijk probleem kan zijn het kiezen van de juiste VM-size en disk-type op basis van de vereisten van de workload. Ook kan het configureren van de Network Security Group voor beveiliging uitdagend zijn als de regels niet correct zijn ingesteld.

## Resultaat
De opdracht is gelukt als de Azure Virtual Machine succesvol is aangemaakt met de gewenste configuratie en eventuele beveiligingsmaatregelen, en de kosten van de VM zijn gecontroleerd voordat deze wordt geïmplementeerd. Screenshots kunnen worden gebruikt om het succes van elke stap te documenteren.

![error](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/fba43c11dfb824da25d65306b49e93618dd3fb23/00_includes/Azure%20week%201/vm/Schermafbeelding%202024-04-30%20113912.png)