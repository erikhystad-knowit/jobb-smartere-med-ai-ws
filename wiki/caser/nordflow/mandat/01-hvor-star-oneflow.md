---
title: 1. Hvor står OneFlow i dag?
type: korpus
case: nordflow
opprettet: 2026-10-22
oppdatert: 2026-10-22
tags: [mandat, status]
kilder: [BOARD-001, BOARD-002, BOARD-003, BOARD-004, BOARD-005, EM-002, EM-008, EM-010, EM-013, EM-016, EM-017, EM-030, EM-032, EM-038, EM-053, EM-054, EM-055, EM-056, EM-059, EM-062, EM-065, EM-066, EM-067, EM-068, EM-074, EM-076, EM-078, EM-083, EM-084, EM-087, EM-089, EM-091, EM-094, EM-098, EM-102, EM-104, EM-108, EM-111, EM-118, EM-130, EM-136, EM-138, EM-140, EM-145, EM-146, EM-147, EM-149, EM-152, EM-154, EM-156, EM-166, EM-167, EM-173, EM-177, EM-178, EM-179, EM-181, EM-182, EM-190, EM-196, EM-201, EM-221, FIN-001, FIN-002, FIN-003, FIN-004, FIN-005, FIN-006, FIN-007, HR-001, HR-002, HR-003, OF-001, OF-002, OF-003, OF-005, OF-007, OF-008, OF-009, OF-010, OF-011, OF-012, OF-013, OF-014, OPS-001, OPS-002, OPS-003, OPS-004, OPS-005, OTHER-001, TECH-001, TECH-002, TECH-003, TECH-004, TECH-005, VEN-001, VEN-002]
---

# 1. Hvor står OneFlow i dag?

## Kort svar

OneFlow står ikke slik styrepakken fra 26. august beskriver det («gul – stabiliserende», 395 mill., ferdig 28. februar 2027) [BOARD-004, BOARD-005]. Finance sin kontrollerte prognose per 16. september er 472 mill. netto (intervall 455–494), mot styrets ramme på 280 mill. [FIN-005, FIN-004, BOARD-002]; 318 mill. var allerede påløpt per 31. august [FIN-005, FIN-007]. Realistisk nordisk ferdigstillelse er juni 2027, ikke februar [TECH-002, FIN-004, TECH-003]. Varige gevinster er korrigert fra 210 til 128 mill. etter at 40 mill. er dobbelttelt mot Cobalt-planen [FIN-006, EM-178]. Samtidig faller kundedriften (SLA 91,4 % mot mål 97,0 %) og fem fornyelser på 146 mill. årlig verdi er flagget, tre av dem med OneFlow-symptomer [OPS-001, OPS-004]. Den tekniske kjernen er likevel levedyktig; hovedproblemet er styring, data og kapasitet, ikke plattformen [TECH-002]. Kildene stopper midt i september; utfallet av styringsgruppens reset-beslutning 22. september er ikke i materialet [OF-014].

## Status per område

Merking: **KJENT** = belagt i kilde (helst primærdata), **PÅSTAND** = noen hevder det, **ANTAKELSE** = slutning (min eller kildens).

### Fremdrift og plan

- **KJENT:** Styret godkjente 18. des. 2024 ramme 280 mill. og sluttdato 31. des. 2026 [BOARD-002]. Styringsgruppen vedtok 18. mars 2026 en intern recovery baseline (28. feb. 2027, 395 mill.) som uttrykkelig *ikke* er ny ramme eller styregodkjent rebaseline [OF-013]. Styret i august lot ramme og formell dato stå uendret [BOARD-005].
- **KJENT:** Milepælsdefinisjonen er endret: «teknisk klar for test» teller nå som lukket milepæl, og bølger kan regnes på plan med redusert utvalg [OF-003, OF-013]. Testen sier selv at «klar for test» ikke er bestått test [EM-016, EM-190].
- **KJENT:** Avvik mot original plan: data/migrering ca. 20 uker, plattform/integrasjon 17 uker (11 mot recovery), prosess ca. 14 uker [OF-008, EM-076, EM-118]. Prosesser godkjent: 9 av 23 [OF-007, EM-118]. Dataobjekter godkjent: 14 av 27 [TECH-004].
- **KJENT:** Bølge 1 er redusert fra 286 til 42 kunder; test kunne ikke anbefale 286: representative testløp fantes for 61 kunder og bare 38 passerte uten alvorlighetsgrad 1–2-feil, og drift tåler maks 50 [EM-083, EM-084, OPS-003]. Nåværende prognose for bølge 3 (Danmark) er 30. juni 2027 mot original 31. des. 2026 [TECH-003, OF-002].
- **PÅSTAND:** Programdirektøren: juni 2027 er «konservativt arbeidsestimat», ikke programdato [EM-089]. Statusfargen er styrt: «Bruk gul på totalen», originalplan flyttet til vedlegg, «detaljene muntlig» [EM-010, EM-013].
- **ANTAKELSE:** PMO foreslår rød samlet status [OF-008]; datalederen kaller data rød og «følger plan» uholdbart [EM-008].

### Økonomi (prognose, kostnad, gevinster)

| Mål | Tall (mill. kr) | Kilde | Dato |
|---|---|---|---|
| Godkjent ramme | 280 | [BOARD-002, FIN-001] | 18.12.2024 |
| Rapportert prognose | 395 | [OF-013, BOARD-004] | mar./aug. 2026 |
| Bottoms-up juni | 438 | [FIN-003] | juni 2026 |
| Bottoms-up august v5 (lav/base/høy) | 455 / 459 / 494 | [FIN-004] | aug. 2026 |
| Kontrollert prognose, netto (brutto 506, kreditt –34) | 472 | [FIN-005] | 16.09.2026 |
| Påløpt / forpliktet / ikke forpliktet | 318 / 91 / 63 | [FIN-005] | 31.08.2026 |

- **KJENT:** Avviket 395→438 er forlengelse (+16 intern, +17 konsulenter, +19 Convergent) og at reserven (17) er fordelt [FIN-003]. Påløpt 318 er allerede 38 over rammen på 280 (min utregning) [FIN-005, BOARD-002].
- **ANTAKELSE:** Om «ramme» omfatter intern tid (78 påløpt) er ikke dokumentert [FIN-007, FIN-001]; sammenlikningen 318 mot 280 må avklares av økonomi.
- **PÅSTAND:** 395 «inkluderer forventet leverandørkreditt» [BOARD-004, CFO i BOARD-005]. Kreditten er «ikke avtalt» [FIN-004]; Nordflows leverandøransvarlig (Ole Martin Kvale) anslår 12 mill. nær sikkert og 12–22 til forhandling [EM-065]. Convergent avviser netto krav på 34 [EM-067].
- **KJENT:** 395 utelater ifølge Finance sannsynlig forlengelse (41), ekstra data/test (22), stabilisering (19) og netto øvrige risikoer (29) [EM-173]. Identifiserte poster ligger i risikovedlegget, ikke i prognosen [BOARD-004].
- **Utenfor programkost:** linjekost 11,2 mill. (overtid, innleie, kreditter, SLA-kreditter) [OPS-002, FIN-007]; kjent og mulig bruttoeksponering i inntekter 27,6 mill., hvorav bekreftet kreditering 3,6 og mulig ikke bokført kontraktseksponering 8,9 (7,2 netto etter overlapp) [OPS-005].
- **Gevinster, KJENT:** Business case: 210 mill. varig fra 2028, 620 mill. kumulativt 2025–29, NPV 218 [FIN-001, BOARD-001]. Korrigert varig gevinst 128 mill., først fra 2029 (–40 dobbelttelling mot Cobalt: 26 bemanning + 14 innkjøp; –42 øvrig nedjustering) [FIN-006, FIN-002, EM-177, EM-178]. Ny NPV og kumulativ gevinst er ikke beregnet; CFO har bedt om sensitivitet [EM-179].
- **Merknad:** I business caset summerer ikke gevinstkomponentene til «Brutto gevinst» i 2025–2027 (f.eks. 0 mot 18 i 2025; 139 mot 121 i 2027) [FIN-001]. NPV-tallet kan ikke etterprøves fra filen.

### Teknologi, migrering og integrasjon

- **KJENT:** 18 av 64 kritiske integrasjoner er ikke produksjonsklare (9. sept.; 21 per 27. juni, 19 per 12. aug.) [TECH-005, EM-098, EM-102]. 14 av 27 dataobjekter består (16 i juni før skjerpede krav) [TECH-004, EM-074, EM-076]. Kundemaster: 11,7 % duplikater mot krav <2,0 %; fakturamottaker mangler/tvetydig i 8,4 % av aktive kontrakter [TECH-004].
- **KJENT:** Leverandørens migreringsverktøy kom fem uker forsinket (6. mai forventet, levert 13. juni med feil) [EM-053, EM-056, VEN-002]. Convergent har byttet løsningsarkitekt to ganger [EM-054, VEN-002]. Nordflow leverte representative testdata 17. juni, over tre uker for sent [EM-108], og 11 designbeslutninger kom 4–9 uker for sent [EM-055].
- **KJENT:** Beslutningskøen: median 35,5 dager mot mål 7; 10 av 12 kritiske saker over 30 dager; seks er fortsatt uten beslutning [OF-011, EM-030].
- **KJENT:** Av de 18 integrasjonene har bare 5 Convergent-feil som hovedårsak i Nordflows tabell [TECH-005]. Plattformen alene kan ikke gjøre migreringen klar [OF-012].
- **PÅSTAND (CIO):** Kjernen er levedyktig; fullføring 30. juni 2027; anbefaler fire ukers kontrollert reset med redusert kjerne [TECH-002, EM-196]. Dokumentet er utkast.
- **Avgrensning:** Systemlandskapet (3 ERP, 4 CRM, 3 portaler, >70 punktintegrasjoner) forklarer behovet, ikke programmets prestasjon [TECH-001].

### Drift og kunder

| KPI | Jan 2026 | Aug 2026 | Mål 2026 | Kilde |
|---|---|---|---|---|
| SLA overholdt | 95,8 % | 91,4 % | 97,0 % | [OPS-001] |
| Førstegangsløsning | 81,6 % | 74,9 % | 84,0 % | [OPS-001] |
| Svartid | 48 s | 132 s | 35 s | [OPS-001] |
| Fakturakorrigering | 2,0 % | 4,9 % | 1,2 % | [OPS-001] |
| Annualisert logo-churn | 5,0 % | 6,7 % | 4,3 % | [OPS-001] |

- **KJENT:** Fallet er størst i enheter som har avgitt erfarne folk til OneFlow, men fravær (7,1 %), sesong og marked bidrar; hele fallet kan ikke tilskrives programmet [OPS-002].
- **KJENT:** Pilot (42 kunder): 17 med manuell fakturakontroll, 8 med portal-/ordreavvik, korreksjonsrate 7,8 %; ingen systematisk havari [OPS-003]. Utvalget er lite [EM-094].
- **KJENT:** Fem fornyelser, 146 mill. årlig verdi: EnergiVest 42 (31.10.2026), Nordbygg 34, Skandia 29, Metrohandel 23 (15.10.2026), Svea 18; tre har OneFlow-signaler (105 mill. etter min summering) [OPS-004, EM-149]. Ledelsen advarer mot å kalle alle 146 «OneFlow-effekt» [EM-149].
- **PÅSTAND:** «Håndterbar», «ingen vesentlig inntektseffekt på konsernnivå» [BOARD-004]. Ingen samlet eier av kunde- og inntektsrisiko er avklart [OF-014, EM-038].
- **ANTAKELSE:** Metrohandel-fornyelsen (15. okt.) er passert i dag; utfallet er ukjent.

### Organisasjon og leverandør

- **KJENT:** Kapasitet uke 35: plan 168 FTE, reell 119, gap 49 (data 21, test/integrasjon 18, prosess 10); 37 over 120 % belastning; 12 avganger [HR-002, EM-130]. Pulsmåling: «planen er realistisk» 36/100, «beslutninger tas raskt nok» 32/100 (svarprosent 71) [HR-003].
- **KJENT:** Linje og program konkurrerer om samme personer uten prioriteringsregel; mandatet sier ikke hvem som avgjør konflikter [HR-001, OF-001]. Prosesseiere var ikke utpekt ved signering [OF-001, OF-002].
- **KJENT:** Operativ tilbaketrekking fra programmet har kostet anslått seks uker i data/test [EM-145]; midlertidig backfill godkjent (maks 1,8 mill., fire uker) [EM-140].
- **PÅSTAND (HR):** Motivasjon er ikke primærårsak til forsinkelsen [HR-003, EM-201].
- **Leverandør:** Kontrakten gir kredittgrunnlag, men ikke grunnlag for å legge hele avviket på én part [VEN-001]. Convergent aksepterer fem ukers forsinkelse og tre feil, men viser til 31 kundeforårsakede hendelser [VEN-002, EM-111, EM-067].

## Det ledelsen rapporterer vs. det dataene viser

| Påstand i ledelsesrapportering | Hva primærkildene viser | Avvik | Kilder |
|---|---|---|---|
| Samlet gul – stabiliserende | Data/prosess røde i RAID; 7 røde risikoer; PMO foreslår rød | Farge vurdert mild | [BOARD-004, OF-010, OF-008] |
| Prognose 395 mill. | Kontrollert 472 netto (455–494) | +77 mill. (+19,5 %) | [BOARD-004, FIN-005] |
| Måldato 28.02.2027 | Juni 2027 (CIO, Finance base) | ca. 4 måneder | [BOARD-004, TECH-002, FIN-004] |
| Første bølge «kontrollert pilot» | 286→42 kunder; korreksjon 7,8 % | Utelatt i lysbilder | [BOARD-004, OPS-003] |
| Kundesituasjon håndterbar | SLA –4,4 pp, churn 6,7 %, 146 mill. i fornyelser | Ikke samlet vist | [BOARD-004, OPS-001, OPS-004] |
| Varig gevinst 184 fra 2028 | 128 fra 2029 | –56 mill./år | [BOARD-003, FIN-006] |
| Plattform «klar for test» | 18 av 64 integrasjoner ikke produksjonsklare | Ny definisjon | [BOARD-004, TECH-005] |
| Leverandør hovedflaskehals | 5 av 18 leverandørfeil (Nordflow) / 6 (CIO) | Delt ansvar | [BOARD-003, TECH-005, EM-104] |
| Kapasitet ikke omtalt | Gap 49 FTE, 37 over 120 % | Utelatt | [BOARD-004, HR-002] |

## Motstrid mellom kilder

> [!konflikt] Motstrid
> [BOARD-004] hevder sluttprognose 395 mill., mens [FIN-005] (nyere) hevder 472 mill. netto. Uavklart per 2026-10-22. FIN-005 er en kontrollert arbeidsbok avstemt mot påløpt/forpliktet [EM-173]; 395 er en intern styringsprognose uten bottoms-up vedlagt [BOARD-003, OF-013], men er fortsatt «siste godkjente» [EM-002].

> [!konflikt] Motstrid
> [EM-166, EM-167] omtaler 382 mill. som tallet i styrepakken, mens [BOARD-003, BOARD-004, OF-013] (alle) bruker 395 mill. Uavklart per 2026-10-22. Forskjellen på 13 mill. er ikke forklart i materialet.

> [!konflikt] Motstrid
> [EM-173] hevder at 395 utelater poster på 41+22+19+29 = 111 mill., mens differansen til netto 472 er 77 mill. ([FIN-005]). Uavklart per 2026-10-22. 111 er forenlig med brutto 506 (395+111), men [BOARD-003] sier at 395 allerede inkluderer kreditt; ANTAKELSE: 395 er i praksis sammenliknet på ulikt kredittgrunnlag.

> [!konflikt] Motstrid
> [OF-007, BOARD-004] hevder 28. februar 2027, mens [TECH-002, FIN-004, TECH-003] (nyere) hevder 30. juni 2027 (base). Uavklart per 2026-10-22. CIO og Finance bygger på verifiserte tellinger; programdirektøren har dokumentert preferanse for å beholde februar [EM-089, EM-010].

> [!konflikt] Motstrid
> [VEN-002] hevder at 5 av 18 integrasjoner er leverandørfeil, 10 kunde-beslutning/data og 3 delt, mens [TECH-005] og [EM-104] (samme dato, 9. sept.) hevder henholdsvis 5/6/4/3 og 6/5/4/3 (Convergent / beslutning / testdata / scope). Uavklart per 2026-10-22. VEN-002 er uttrykkelig en leverandørposisjon med kommersiell egeninteresse.

> [!konflikt] Motstrid
> [VEN-002] hevder at Convergent er villig til å diskutere kreditt på 24–34 mill. (betinget av scope-frys), mens [EM-067] (nyere) sier de avviser et netto krav på 34. [EM-062] tilskriver intervallet 24–34 Nordflows eget krav. Uavklart per 2026-10-22. Ingen skriftlig avtale finnes [FIN-004].

> [!konflikt] Motstrid
> [EM-147] (17. aug., foreløpig) navngir de fem fornyelseskundene som Fjordkraft Drift, ScanMarine, MedicoLog, Vestbygg og Arctiq, mens [OPS-004] (12. sept.) navngir EnergiVest, Nordbygg, Skandia, Metrohandel og Svea; begge oppgir 146 mill. ([EM-146, OPS-004]). Uavklart per 2026-10-22. OPS-004 er primærrapport og nyere; ulikheten kan være ulikt utvalg.

> [!konflikt] Motstrid
> [OPS-003, EM-091] hevder at 17 av 42 pilotkunder krevde manuell fakturakontroll, mens [EM-078] hevder at alle 42 ligger i manuell fakturakontroll. Uavklart per 2026-10-22. ANTAKELSE: alle 42 er i kontrollregime, 17 hadde korreksjonsbehov.

> [!konflikt] Motstrid
> [TECH-003] hevder bølge 1-cutover er prognosert 18. des. 2026 (42 av 286 valgt), mens [OPS-003, EM-087] viser at piloten på 42 allerede er migrert og analysert (34 av 42 stabilisert 18. aug.). Uavklart per 2026-10-22. Hvilke kunder som omfattes av hvilken bølge er ikke avklart.

> [!konflikt] Motstrid
> [BOARD-003, EM-066] hevder at leverandørsvikten er hoveddriver, mens [TECH-002, EM-108, EM-059] hevder delt ansvar og at Nordflows beslutninger og testdata også forsinker. Uavklart per 2026-10-22. CIO og testleder har ikke leverandøregeninteresse; Nordflows leverandøransvarlig har forhandlingsinteresse.

Kandidater til tidsforskjell, ikke reell motstrid: ordre >45 dager 13,9 (28.8.), 16,8 (2.9.), 16,5 (11.9.) [EM-152, EM-154, EM-156, OPS-005]; linjekost 8,7 (14.8.) mot 11,2 [EM-138, OPS-002]; SLA juli 92,1 mot august 91,4 [EM-136, OPS-001].

## Kildekvalitet

- **Sterk (primærdata):** FIN-005 (kontrollert, avstemt), FIN-006 (avstemt og bekreftet av to ledere [EM-178, EM-179]), OPS-001, OPS-005, TECH-004, TECH-005, HR-002, OF-010, OF-011, BOARD-002, BOARD-005 (protokoller).
- **Middels:** FIN-003/FIN-004 (arbeidsfiler, ikke kontrollert, kreditt antatt); OPS-003 og OPS-004 (små utvalg); TECH-002 (CIO-utkast, ny i rollen, anbefaler reset [HR-001, OF-013]).
- **Svak/egeninteresse:** BOARD-003, BOARD-004, OF-007 og OF-005 er ledelsesoppsummeringer der e-postene viser redigering av budskap [EM-010, EM-013, EM-017]. VEN-002 er leverandørposisjon. CFO ønsket å avvente ny prognose før bankmøtet [EM-182, EM-181], noe som gir egeninteresse i tidspunkt for tall.
- **Gjeldende versjoner:** FIN-005 (16.9.) > FIN-004 (v5) > FIN-003; FIN-006 v3 for gevinst; OF-010 (31.8.) > OF-009; BOARD-004 (ENDELIG) > BOARD-003; OF-008 er nyest (14.9.) men uten godkjenning.
- **Støy (ikke relevant):** Aurora (0,6 FTE), lokaler, ESG, utstyr, reiser og sosiale arrangementer [OTHER-001, EM-221].
- **Mangler:** Original plan og bottoms-up som vedlegg til styret [BOARD-003]; kontrakt mot lovet kreditt; alt etter 17. sept.

## Usikkerhet og hull

- Utfall av 22. september (reset, scope-frys, kreditt) og styremøte: ikke i materialet [OF-014, EM-032]. Trengs: referat, oppdatert FIN-fil.
- Reell kredittstørrelse: trenger skriftlig tilbud [EM-068].
- Om rammen 280 omfatter intern tid; trenger avgrensning fra Finance [FIN-007].
- Ny NPV og kumulativ gevinst med 128 mill. fra 2029 [EM-179].
- Samlet kunde- og inntekteffekt, inkl. utfall av fornyelser per 15./31. okt. [OPS-004].
- Hvem som eier scope-, kunde- og inntektsrisiko [OF-014].
- Banksituasjon: covenant holder ved 470, men headroom lavere Q1/Q2 [EM-181]; ikke dokumentert utover foreløpig modell.

## Nøkkelkilder

1. [FIN-005] – kontrollert prognose 472 med påløpt/forpliktet.
2. [FIN-006] – gevinstavstemming 210→128.
3. [TECH-005] – de 18 integrasjonene etter årsak.
4. [TECH-002] – CIO-vurdering og anbefaling.
5. [TECH-004] – datakvalitet med tallene.
6. [OPS-001] – KPI-utvikling i kundedrift.
7. [OPS-004] – fornyelser på 146 mill.
8. [OF-010] – RAID 31. aug., sju røde risikoer.
9. [OF-011] – beslutningskø.
10. [BOARD-005] – hva styret faktisk vedtok.
11. [EM-010] – instruks om statusfarge og vedlegg.
12. [VEN-002] – leverandørens syn.

## Bidrag til leveranser

- **CEO-brief:** Åpne med 472 (455–494) mot 395 og 280, påløpt 318, juni 2027 [FIN-005, TECH-002]; bruk KJENT/PÅSTAND/ANTAKELSE; si at kilder stopper 17. sept.
- **CEO-brief:** Gevinst 128 fra 2029 (40 dobbelttelt, 42 nedjustert) og at NPV må regnes om [FIN-006, EM-179].
- **Lederpresentasjon:** Vis rapport-vs-data-tabellen; ikke «leverandøren alene»: 5–6 av 18 integrasjoner er leverandørfeil [TECH-005, EM-104].
- **Lederpresentasjon:** Kundeside: 146 mill. i fornyelser (tre med OneFlow-signaler), SLA 91,4 %, og ingen samlet eier [OPS-004, OPS-001, OF-014].
- **90-dagersplan:** Beslutningsrett og 72-timers frist, beskyttet kapasitet (gap 49), portkriterier for data/prosess før bølge 2, og ny styresak om ramme og dato i tråd med vedtak 5 [OF-011, HR-002, TECH-002, BOARD-005].
