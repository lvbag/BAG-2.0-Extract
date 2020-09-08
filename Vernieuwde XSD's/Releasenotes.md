Door signalen van afnemers zijn wij tot de ontdekking gekomen dat de versie van GML welke gebruikt wordt voor het aanmaken van het BAG 2.0 Extract achterhaald was.
Aangezien het BAG 2.0 Extract nog niet volledig was ontwikkeld, is ervoor gekozem om dit en een paar andere kleine wijzigingen aan te passen in de XSD's. Voordat er is besloten om 
de XSD's aan te passen is er uitvraag gedaan onder een groep afnemers naar de impact van deze wijzigingen. Hier is uitgekomen dat de wijzigingen in de XSD's relatief eenvoudig door te 
voeren zijn en weinig impact hebben.

In de nieuwe XSD's zijn de volgende onderdelen gewijzigd:  
  
•	Xlink is vervangen door ObjectenRef een attribuut domein met een vaste waarde. De relatie tussen de verschillende objecten wordt aangeduid door de invulling van het type ObjectRef.  
Voorbeeld: <Objecten-ref:WoonplaatsRef domein="NL.IMBAG.Woonplaats">3560</Objecten-ref:WoonplaatsRef>  

•	De XSD over GML is eenvoudiger opgenomen. In de vorige versie van de XSD’s was veel informatie over het uitleveren van GML 3.2.1. opgenomen die niet van toepassing was op het BAG 2.0 Extract. Al deze overbodige data is vervangen door een GML XSD welke specifiek op Kadaster producten van toepassing is. De gewijzigde XSD is ontwikkeld op basis van GML versie 3.2.2.  

•	Het gebruik van de NEN3610 norm is opgenomen zoals deze bedoeld was en is daardoor gelijk getrokken met het gebruik van de NEN3610 in de BAG API. In de oude versie van de XSD’s was de NEN3610 norm opgenomen in een element. In de nieuwe versie is het een complextype geworden met een attribuut domein met een vaste waarde.  
Voorbeeld: <Objecten:identificatie domein="NL.IMBAG.Woonplaats">3560</Objecten:identificatie>  

•	In alle XSD’s is de namespace versie gewijzigd van 20180601 naar 20200601
