# BAG-werkbank: data

Databestanden voor de [BAG-werkbank](https://josephinelinders.nl/bagwerkbank.html) van het Open Data Atelier (Josephine Linders).

- `index.json`: per gemeente naam, aantallen en bestandsgrootte, met de stand van de BAG.
- `gm/<gemeentecode>.txt.gz`: per gemeente elk adresseerbaar object (verblijfsobject, ligplaats, standplaats) met het hoofdadres, BAG-ID's (ook van openbare ruimte en woonplaats), status, gebruiksdoel, oppervlakte, bouwjaar, pand, wijk, buurt en coördinaten (RD). Gecomprimeerd, compact formaat (formaat 2 sinds november 2026); de werkbankpagina pakt het uit en maakt er ook de download in GGM-vorm van.

**Bron:** Basisregistratie Adressen en Gebouwen (BAG), Kadaster, via PDOK (landelijk GeoPackage, CC0); wijk- en buurtindeling CBS via PDOK (CC BY 4.0). Afgeleid bestand, geen authentieke BAG.

**Verversing:** maandelijks. Deze repository krijgt bij elke verversing een nieuwe geschiedenis; oude standen worden niet bewaard.

© Josephine Linders voor de bewerking. Gebruik van de lijsten in eigen werk mag, met de BAG als bron.
