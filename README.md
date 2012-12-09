attskrivajuridik-csl
====================
A CSL style for Swedish legal writing.

Attskrivajuridik-csl är en CSL-stilmall för svenska rättsvetenskapliga texter.

Stilen är anpassad för [CSL 1](http://citationstyles.org/), som har stöd i flera källhanteringsprogramvaror, bland andra Zotero, Mendeley, Papers och Qiqqa. Som antyds av namnet baserar den sig på instruktionerna för källangivelser i Jensen, Rylander, Lindblom, *Att skriva juridik*, fjärde upplagan. 

Stilmallen är inte komplett utan är i dagsläget anpassad för hänvisningar till lagförarbeten, rättsfall, monografier, avsnitt ur böcker, webbsidor och tidskriftsartiklar.

I detta dokument anges bland annat hur inmatningarna i källhanteringsprogrammet ska ske för att källhänvisningarna ska se så bra ut som möjligt.

Önskemål om kompletteringar och rättelser kan göras genom att anmäla en [Issue](https://github.com/krevad/attskrivajuridik-csl/issues) på GitHub eller genom att du helt enkelt gör en *fork* av stilmallen och gör ändringarna själv och skickar en hämtningsförfrågan (pull request) till detta projekt när du är färdig med ditt ändringsförslag.

# Särskilda anmärkningar
## Förkortningsmarkering
I svenska texter kan förkortningar markeras med en punkt, såsom i exemplet *prop.* för proposition. Denna metod används även i denna stilmall.
## Sortering i källförteckningen
I rättsvetenskapliga texter brukar källförteckningen sorteras på det sättet att åberopat offentligt tryck finns under en särskild rubrik, medan övrig litteratur får en annan rubrik. Ibland förekommer också att åberopade rättsfall ges en särskild rubrik i källförteckningen.

Nuvarande CSL-standard har tyvärr inget stöd för sådan komplex sortering, utan där sker i huvudsak sortering strikt alfabetiskt eller kronologiskt med olika varianter. Eftersom sortering efter författare är den vanligaste metoden i rättsvetenskapliga arbeten är detta också vad som valts i denna mall. Det blir visserligen fel, men förhoppningsvis minst fel. Givetvis går det att manuellt sortera sina källor vilket förmodligen är en ganska enkel uppgift i skrivandets absoluta slutskede.

Förarbeten och rättsfall sorteras emellertid först och skiljs därmed från övriga källor. Däremot kommer alla förarbeten respektive rättsfall att sorteras i alfabetisk ordning vilket många gånger kräver manuell sortering för att de ska hamna rätt.

Vill man ha automatisk uppdelning av sin källförteckning är man hänvisad till källhanteringsprogrammets funktioner för skapande av källhänvisningar.

# Hur mallen installeras
## Zotero
1. Ladda hem stilmallen.
2. Inställningar... > Fliken Källhänvisa > Fliken Stilar > +-knappen > Välj den nedladdade mallen.

# Hur mallen används
Begrepp från den svenska översättningen av Zotero kommer att användas här för översiktlighetens skull, den engelska frasen förekommer ibland inom parentes.

## Allmänt
Vad som ska anges i de olika fältet är ofta klart med hänsyn till fältets namn. Fält som *titel*, *författare* och *ISSN* kommer inte att kommenteras fortsättningsvis om det inte finns särskilda skäl för det.

I fotnoterna kommer allmänt den *korta titeln* att användas. Den fullständiga titeln förekommer bara i källförteckningen.

## Böcker (Book)
CSL-standarden har en särskild kategori för avhandlingar. I denna stilmall jämställs de med böcker.
## Bokavsnitt (Book Section)

## Artiklar
### Vetenskapliga tidskrifter (Journal Article)
De svenska rättsvetenskapliga tidskrifterna har i allmänhet välkända förkortningar som ska användas vid källhänvisningen. JT (Juridisk tidskrift), SvJT (Svensk juristtidning) och ERT (Europarättslig tidskrift) är några exempel. Ange tidskriftens fullständiga namn i fältet *publikation* medan förkortningen skrivs in i fältet *tidsskriftsförkortning*.

De sidor som artikeln omfattar, alternativt, den sidan artikeln börjar anges i fältet *sidor*.

När tidskriften pagineras löpande inom samma årgång är *nummer*, det vill säga i vilket häfte artikeln tryckts, inte en nödvändig uppgift.

### Nyhetstidning, dagspress (Newspaper Article)

### Annan tidning (Magazine Article)

## Rättsfall (Case)
CSL har en egen kategori för rättsfall. Många av de fält som används är anpassade efter det amerikanska rättsystemet vilket innebär att många fält saknar motsvarighet för svenska rättsfall men också rättsfall från EU-domstolen och Europadomstolen.

### Svenska rättsfall

#### Refererade fall
Refererade fall från svenska domstolar följer i allmänhet en serie, NJA-serien för Högsta domstolen, HFD-serien från Högsta förvaltningsdomstolen, AD-serien för Arbetsdomstolen, och så vidare.

I NJA-serien åtskiljs rättsfallen med sidnummer, medan de flesta andra serier rättsfallsreferat använder löpnummer.

I fältet *x* anges *x*.
I fältet *y* anges *y*.

#### Orefererade fall

Orefererade fall förekommer ibland som notisfall, då finns en praxis för hur man hänvisar till dessa. I andra fall anges domstolens namn och målnummer.

### EU:s domstolar
För utländska rättsordningar gäller i allmänhet de citeringsregler som allmänt gäller där. För svensk del lär EU-domstolens och Europadomstolens avgöranden vara vanligast förekommande.

I källhänvisningen bör hela referensen anges, och nödvändiga uppgifter är målnummer, parterna i målet, och målets plats i rättsfallssamlingen.

Här kan det vara värt att notera att den tidigare förekommande förkortningen REG (Rättsfallssamling för Europeiska gemenskaperna) sedan Lissabonfördraget har ersatts med REU (Rättsfallssamling för Europeiska unionen).

### Europadomstolen
Europadomstolens domar anges med parter och datum.

I fältet *x* anges hela namnet.
I fälet *kortnamn* anges parterna.

## Lagförarbete (Bill)
Översättningen av det engelska *bill* till *lagförarbete* är egentligen inte helt klar, men rimlig i svensk kontext eftersom fler texter än just propositionen är relevanta här.

Lagförarbeten används inte bara för propositioner, utan även utredningar (SOU, Ds), riksdagsmotioner och utskottsbetänkanden.

Såsom *sponsor* anges motionsförfattare.
Såsom *session* anges riksdagsår, om nödvändigt.
Såsom *lagstiftare* anges det organ som utfärdat förarbetet i fråga.

*xxx-nummer* är referensnumret för förarbetet, exempelvis *Prop. 2006/07:5* eller *SOU 2009:24*.

Ett alternativ till att använda lagförarbete kan vara att ange källan som ett dokument. Detta kan dock få betydelse för hur referensen sorteras i källförteckningen.

## Författning (Statute)
Det sätt CSL förutsätter att författningar matas in passar inte så väl med svenska författningar.

Författningens namn: Lag (1915:218) om avtal och andra rättshandlingar på förmögenhetsrättens område  
Kortnamn: AvtL

## Hemsida (Webpage)
Såsom *titel på webbplats* anges webbplatsens namn, exempelvis *Dagens nyheter*.
Glöm inte att ange när informationen är hämtad.
