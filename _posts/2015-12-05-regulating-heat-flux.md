---
layout: post
title: Regulating Heat Flux
date: 2015-12-05
categories: [wave equations, regulation]
---
# Regulating Heat Flux in Fire #

### Regulering av varmefluks i brannforsøk ###
 
####Kort om SP Fire Research:####
SP Fire Research AS (SPFR) (tidligere SINTEF NBL – Norges branntekniske laboratorium) er et aksjeselskap eid av SP Sveriges Tekniska Forskningsinstitut (70 %) og SINTEF (30 %).  Sammen med svenske SP Fire Research-avdelingen er vi et av verdens største branntekniske kompetansesenter. Vi har omfattende forsøksressurser ved vårt laboratorium på Tiller og vi jobber mot alle samfunnssektorer og industrier hvor brann utgjør en risiko. For mer informasjon, se www.spfr.no.
 
####Problemet:####
For å teste passiv brannbeskyttelse og konstruksjoner som skal brukes på offshoreinnretninger eller i andre industrier hvor man har fare for utslipp av brennbar gass eller væske med høyt trykk, gjennomføres det såkalte jetbranntester (antent høytrykksutslipp). Dette gjøres i utgangspunktet i henhold til ISO 22899-1 eller OTI 95634. Disse teststandardene angir propantrømningsrate på 0,3 kg/s, og selv om standardene ikke stiller noen krav til varmefluks i disse testene, oppnår man ca. 250 kW/m2. Vår forskning viser imidlertid at man i enkelte tilfeller kan få langt høyere flukser i reelle branntilfeller, -noe som vil si at de etablerte teststandardene ikke er dekkende for disse tilfellene.  
 
Som et svar på dette har SPFR videreutviklet en testmetode, som baserer seg på de nevnte standardene.  Vår variant gir høyere flukser enn standarden, og vi har et definert mål om å holde fluksnivået på 350 kW/m2 (tilsvarer temperaturer rundt 1300 °C for et svart legeme). Det har imidlertid vist seg at det er ikke-trivielt å holde fluksnivået noenlunde konstant. Per i dag styrers fluksnivået ved å justere propanstrømningsrate og lufttilførsel. Selv om man oppnår tilnærmet steady-state, kan temperaturen tilsynelatende uprovosert enten stige eller synke kraftig. Enkelte av disse endringene kan komme av at prøvestykket, eller brannbeskyttelsen, endrer seg under testen.
 
Testoppsettet består av en ovn, -en kube med sider på ca. 3 m. Prøvestykket som skal testes plasseres i ovnen, og blir utsatt for en jet med antent propangass. Prøvestykket blir dermed utsatt for høye temperaturer og erosjonskraften fra gasstrålen.
 
Temperaturene som oppnås i ovnen er avhengige av:
* Mengde gass (i testene ca. 0,3 kg/s)
* Tilgjengelig oksygen (har regulerbare vifter i testene)
* Vind og værforhold
* Prøvestykket som testes
* Fuktinnhold i selve ovnskonstruksjonen (ovnen er bygd av siporex (porebetong))
 
I forsøkene er følgende målinger tilgjengelige:
* Temperaturer i ovnen
* Omgivelsestemperatur
* Gasstrømningsrate
* Pådrag på vifter (%)
* Vindmåling (styrke og retning)
* Andre målinger vil vurderes ved behov
 
En reguleringsteknisk utfordning er at systemet har en forholdsvis lang tidskonstant (fra ≈20 sek – 2 min).
 
 
####Oppgave:####
·         Sette seg inn i problemstillingen.
o   Forenklet forbrenningslære.
o   Mekanismer for varmeoverføring.
§  Stråling
§  Konveksjon
§  Ledning
o   Demonstrasjon av jetbranntest.
·         Lage en matematisk modell som kan beskrive systemet og dets respons.
·         Kalibrere modellen mot historiske måledata.
·         Utvikle en regulator som kan holde fluksen på ønsket nivå, og som tar hensyn til, og kompenserer for, endringer i betingelser under test.
·         Implementering og uttesting av regulator i brannforsøk i redusert skala, -og deretter i fullskala.
 
Resultatene fra oppgaven vil være konfidensielle.
