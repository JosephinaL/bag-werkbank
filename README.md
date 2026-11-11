# BAG-werkbank: data

Databestanden voor de [BAG-werkbank](https://josephinelinders.nl/bagwerkbank.html) van het Open Data Atelier (Josephine Linders).

- `index.json`: per gemeente naam, aantallen en bestandsgrootte, met de stand van de BAG.
- `gm/<gemeentecode>.txt.gz`: per gemeente elk adresseerbaar object (verblijfsobject, ligplaats, standplaats) met het hoofdadres, BAG-ID's (ook van openbare ruimte en woonplaats), status, gebruiksdoel, oppervlakte, bouwjaar, pand, wijk, buurt en coördinaten (RD). Gecomprimeerd, compact formaat (formaat 2 sinds november 2026); de werkbankpagina pakt het uit en maakt er ook de download in GGM-vorm van.
- `bouw/<gemeentecode>.json.gz` en `bouw/index.json`: per gemeente de panden in de bouwstroom (bouwvergunning verleend, bouw gestart, in gebruik niet ingemeten, sloopvergunning verleend, en in gebruik met bouwjaar vanaf vorig jaar), ook zonder verblijfsobject, met hun vlak (WGS84) en verblijfsobjecten, plus nieuwe verblijfsobjecten in bestaande panden. Gemeente van een pand op ligging, van een verblijfsobject op bronhouder. Gebruikt door [Bouwstroom](https://josephinelinders.nl/bouwstroom.html).
- `label/<gemeentecode>.json.gz` en `label/index.json`: per gemeente en buurt het aantal woningen en utiliteitspanden naar energielabel (nu en op 1 juli 2022), zonder rijksmonumenten, met het aandeel huurwoningen per buurt, en per utiliteitspand met label D, E, F of G het adres en het label. Geen gegevens per woning. Gebruikt door de [Energielabelkalender](https://josephinelinders.nl/energielabelkalender.html). Deze bestanden zijn er voor die pagina. Ze zijn niet bedoeld om eigenaren of gebruikers van gebouwen te benaderen; zie [Gegevens over gebouwen](https://josephinelinders.nl/colofon.html#gebouwen).

**Bron:** Basisregistratie Adressen en Gebouwen (BAG), Kadaster, via PDOK (landelijk GeoPackage, CC0); wijk- en buurtindeling CBS via PDOK (CC BY 4.0). Voor `label/` ook: energielabels per pand van het RIVM (afgeleid uit EP-Online van RVO, Public Domain Mark 1.0), rijksmonumenten van de RCE via PDOK (CC BY 4.0) en CBS Kerncijfers wijken en buurten (CC BY 4.0). Afgeleide bestanden, geen authentieke BAG.

**Verversing:** maandelijks. Deze repository krijgt bij elke verversing een nieuwe geschiedenis; oude standen worden niet bewaard.

© Josephine Linders voor de bewerking. Gebruik van de adreslijsten (`gm/`) en de bouwbestanden (`bouw/`) in eigen werk mag, met de BAG als bron. Voor `label/` geldt de beperking hierboven.
