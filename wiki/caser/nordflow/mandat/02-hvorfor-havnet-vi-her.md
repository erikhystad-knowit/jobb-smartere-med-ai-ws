---
title: 2. Hvorfor har vi havnet her?
type: korpus
case: nordflow
opprettet: 2026-10-22
oppdatert: 2026-10-22
tags: [mandat, arsaker]
kilder: [BOARD-001, BOARD-002, BOARD-003, BOARD-004, BOARD-005, EM-008, EM-010, EM-011, EM-013, EM-016, EM-020, EM-024, EM-025, EM-027, EM-030, EM-035, EM-038, EM-040, EM-043, EM-044, EM-046, EM-050, EM-052, EM-053, EM-054, EM-055, EM-056, EM-066, EM-067, EM-069, EM-072, EM-085, EM-099, EM-102, EM-104, EM-105, EM-108, EM-116, EM-117, EM-124, EM-125, EM-127, EM-130, EM-141, EM-143, EM-145, EM-146, EM-147, EM-166, EM-167, EM-168, EM-173, EM-177, EM-178, EM-181, EM-182, EM-186, EM-197, EM-199, EM-202, FIN-002, FIN-003, FIN-004, FIN-005, FIN-006, FIN-007, HR-001, HR-002, HR-003, OF-001, OF-002, OF-003, OF-004, OF-006, OF-007, OF-008, OF-009, OF-010, OF-011, OF-012, OF-013, OF-014, OPS-001, OPS-002, OPS-003, OPS-004, OPS-005, OTHER-001, TECH-001, TECH-002, TECH-004, TECH-005, VEN-001, VEN-002]
---

# 2. Hvorfor har vi havnet her?

## Kort svar

OneFlow er forsinket og dyrere enn vedtatt fordi programmet ble startet og drevet uten at vedtatte forutsetninger var på plass, og fordi ingen kunne avgjøre uenigheter raskt nok. Fire rotårsaker er best belagt: (1) bygg startet før prosesseiere, datakvalitet og testdata var sikret, på et business case med uavstemte gevinster [BOARD-002, OF-001, OF-002, FIN-006]; (2) uklar beslutningsrett, med median 35,5 dager på kritiske beslutninger mot mål 7 [OF-011, OF-001]; (3) vekst i endringer og lokale krav uten uttak av scope [EM-043, EM-046]; (4) kapasitet som aldri ble skjermet mellom linje og program, 119 tilgjengelig mot 168 planlagt [HR-002]. Leverandøren er en reell, men sekundær forsterker. Rapporteringen (gul status, 395 mill.) har forsinket korreksjon og er forsterker, ikke årsak [BOARD-004, FIN-005]. Sluttkostnad er nå vurdert til 472 mill. netto (455–494) mot en vedtatt ramme på 280 mill. [FIN-005, BOARD-002].

## Rotårsaker

**Skala:** KJENT = belagt i primærdata. PÅSTAND = noen hevder det. ANTAKELSE = slutning om årsak. Selve årsakskjedene er antakelser; belegget gradert under.

### R1. Start uten verifiserte forutsetninger og med uavstemt business case

- **Påstand (antakelse):** Planen (ferdig 31.12.2026, 280 mill.) var urealistisk fra dag én fordi portkravene ble hoppet over. **Belegg: sterkt.**
- **KJENT:** Styret vedtok 18.12.2024 ramme 280 mill., varig gevinst 210 mill./år fra 2028 og kalte prosesseierskap og datakvalitet «portkriterier, ikke aktiviteter» [BOARD-001, BOARD-002]. Dataomfang, lokale kontraktsvarianter og linjekapasitet var «ikke endelig verifisert» [BOARD-001]. Ved godkjenning var prosesseiere «ikke startet» og dataprofilering 22 % kartlagt; alle spor startet parallelt i januar 2025; mobilisering planlagt seks uker, oppstart etter tre [OF-001, OF-002]. Full profilering (mars 2026) ga 12,4 % duplikater mot krav under 2 %; i august 11,7 % [EM-072, TECH-004]. Camilla Bruun advarte mot å låse dato før hele uttrekket var analysert [EM-069] og skrev senere at dato ble satt før kvalitetskriterier [EM-186].
- **Gevinstsiden:** 40 av 210 mill. er dobbelttelt mot Cobalt-planen (26 bemanning, 14 innkjøp) og 42 mill. er øvrig nedjustering; korrigert varig gevinst er 128 mill. fra 2029 [FIN-006, FIN-002, EM-178]. Styret ba i 2024 om avstemming, men det ble ikke fremlagt [BOARD-002].
- **Årsakskjede:** udefinerte eiere og uren data gir uferdige krav og regler, som gir integrasjoner og migrering som ikke kan testes, og dermed forsinkelse og omarbeid.
- **Motbevis:** hvis tilsvarende kostnadsvekst oppstod også da eiere og data var på plass, eller hvis en uavhengig kritisk-sti-analyse viser at forsinkelsen skyldes noe annet.

### R2. Uklar beslutningsrett og styring

- **Belegg: sterkt.**
- **KJENT:** Mandatet angir ikke hvem som avgjør konflikter mellom prosesseiere, program og land; matrisen gir ingen prioritet mellom linje og program [OF-001, HR-001]. Av 12 kritiske beslutninger er median 35,5 dager mot mål 7; seks er fortsatt åpne [OF-011]. Fire prosesser stod uten beslutning 36–52 dager, to av dem fordi beslutningsretten var uavklart [EM-116, EM-117]. Reset-notatet og scope-frys er utsatt av samme spørsmål [EM-035, OF-014]. Ingen samlet eier av kunde- og inntektsrisiko [EM-038, OF-010].
- **Årsakskjede:** åpne beslutninger blokkerer kontraktsmodell, testdata og integrasjoner. Av 18 integrasjoner som ikke er produksjonsklare venter 6 på Nordflow-beslutning og 4 på testdata [TECH-005, OF-012].
- **Motbevis:** hvis beslutninger med navngitt eier også tar over 7 dager, eller hvis de sene beslutningene ikke lå på kritisk sti.

### R3. Uavklart scope: endringsvekst og lokale krav

- **Belegg: middels** (tallene er PMOs foreløpige estimat).
- **KJENT:** 28 endringsønsker i prosessløpet september 2025 [EM-040]; november 2025: 47 endringer, 19 med full analyse, foreløpig effekt 63 400 timer og 38 mill. [EM-043]. Siste pakker ble godkjent uten full konsekvensanalyse, og ingen funksjonalitet ble tatt ut [EM-046]. Fire danske kontraktspunkter regnes som reelle krav, mens øvrige ønsker ikke har funnet lov- eller kontraktsgrunnlag [EM-124].
- **PÅSTAND:** mange endringer er nødvendige for business caset [EM-044].
- **Årsakskjede:** nye varianter hver uke gjør at de 23 prosessene ikke kan signeres; bygg og test omarbeides [EM-050, OF-011].
- **Motbevis:** hvis endringene vises å ha minimal kritisk-sti-effekt, eller hvis alle var kontrakts- eller lovpålagte.

### R4. Kapasitet ikke skjermet mellom linje og program

- **Belegg: middels til sterkt.**
- **KJENT:** Plan 168 FTE mot bekreftede 126 allerede i februar 2026 på grunn av dobbeltallokering [EM-127]. Uke 35: tilgjengelig 119, gap 49, 37 personer over 120 % belastning, 12 avganger [HR-002, EM-130]. Gapet er størst i data (21) og test/integrasjon (18) [HR-002].
- **Årsakskjede:** erfarne personer trekkes mellom to ledere, noe som forsinker data og test og samtidig svekker drift (se symptomer).
- **PÅSTAND:** tilbakeføringer siden mai har kostet «estimert seks uker» i data/test [EM-145]. Dette er Håkon Bergs anslag og er ikke dokumentert.
- **Motbevis:** hvis forsinkelsen er like stor på spor uten kapasitetsgap, eller hvis backfill ikke forkorter planen.

## Forsterkere

| Forsterker | Hvordan den gjorde det verre | Kilde |
|---|---|---|
| Recovery-baseline mars 2026 | Ny dato 28.2.2027 og prognose 395 mill. uten styrebehandling; milepæler målt som «teknisk klar for test» i stedet for godkjent leveranse; forutsetninger (7-dagers beslutninger, stabile krav, linjekapasitet) ble ikke innfridd | [OF-003, OF-013, EM-016, EM-024] |
| Rapportering | Gul totalstatus selv om data/migrering var rød; originalplan flyttet til vedlegg; pilotkutt 286 til 42 ikke nevnt for styret; bottoms-up 438 (17.6.) ikke i styrepakke 24.6. | [EM-010, EM-011, BOARD-003, BOARD-004, EM-167, EM-168] |
| Ønske om å unngå ny rebaselining | «Unngå enda en offentlig rebaseline»; sensitivitet holdt internt før bankmøtet | [EM-020, EM-182, EM-181] |
| Leverandør | Migreringsverktøy fem uker forsinket, to arkitektbytter, 5–6 feil i integrasjoner. Nordflow forsinket selv representative testdata til 17.6. og leverte beslutninger 4–9 uker sent | [EM-055, EM-054, EM-108, VEN-002] |
| Ressurstrekk fra program til drift | Fire spesialister og tre testressurser tilbake i mai, igjen i juli | [EM-141, EM-143] |
| Åpne beslutninger om reset | Reset utsatt til 22.9.; scope-frys uten klar myndighet | [OF-014, EM-035] |

Bakgrunn som ikke er årsak: Cobalts fragmenterte systemlandskap (3 ERP, 4 CRM, over 70 punktintegrasjoner) forklarer behovet, ikke forsinkelsen [TECH-001]. Project Aurora bruker om lag 0,6 FTE arkitekt og forklarer ikke forsinkelsene [OTHER-001].

## Symptomer

| Symptom | Tall | Peker på |
|---|---|---|
| Kostnad over ramme | Ramme 280 mill.; rapportert 395; bottoms-up juni 438; kontrollert 16.9.: 472 netto (506 brutto, kreditt 34) [BOARD-002, FIN-003, FIN-005] | R1, R2, R3 |
| Dato | Rapportert 28.2.2027; CIO 30.6.2027; base i prognose 30.6.2027 [BOARD-004, TECH-002, FIN-004] | R1, R2, R3 |
| Spor bak | 9 av 23 prosesser signert; 14 av 27 dataobjekter; 18 av 64 integrasjoner ikke klare [OF-007, TECH-004, TECH-005] | R1, R2 |
| Pilot | Bølge 1 redusert fra 286 til 42 kunder; 17 med manuell fakturakontroll; korrigeringsrate 7,8 % [OPS-003] | R1 (data), R2 |
| Drift | SLA 95,8 % (jan) til 91,4 % (aug) mot mål 97,0; svartid 48 til 132 sek. [OPS-001] | R4 (også fravær 7,1 % og sesong [OPS-002]) |
| Kunder | Churn 5,0 % til 6,7 %; fornyelser for 146 mill./år i risiko, tre av fem med OneFlow-signaler [OPS-001, OPS-004] | R4, R1 (indirekte) |
| Faktura | Korrigering 2,0 % til 4,9 %; bekreftet kreditering 3,6 mill.; mulig eksponering 8,9 mill. (7,2 etter overlapp) [OPS-001, OPS-005] | R1 (data) |
| Team | Puls: «planen er realistisk» 36/100; «beslutninger tas raskt nok» 32/100 [HR-003] | R2, R4 |
| Gevinst | 210 til 128 mill./år [FIN-006] | R1 |

## Hendelsesforløp

| Dato | Hendelse | Hvorfor det betyr noe | Kilde |
|---|---|---|---|
| 2024-12-18 | Styret godkjenner 280 mill., slutt 31.12.2026; krever eierskap og datakvalitet som porter | Forutsetninger kjent og ikke verifisert | [BOARD-001, BOARD-002] |
| 2025-01 | Alle spor starter parallelt; prosesseiere ikke utpekt, data 22 % kartlagt | R1 og R2 legges inn i designet | [OF-001, OF-002] |
| 2025-09-18 | 28 endringsønsker i prosessløpet | Scope vokser | [EM-040] |
| 2025-10-21 | Dataansvarlig advarer mot å låse dato | Varsel ble ikke fulgt | [EM-069] |
| 2025-11-09 | 47 endringer, 63 400 timer/38 mill. foreløpig | R3 tallfestet | [EM-043] |
| 2025-11-24 | Siste pakker godkjent uten full analyse | Ingen scope tatt ut | [EM-046] |
| 2026-01 | Status gul, original dato holdes | Avvik utsettes | [OF-004] |
| 2026-02-08 | 168 planlagt mot 126 bekreftet FTE | R4 | [EM-127] |
| 2026-03-18 | Recovery baseline: 28.2.2027, 395 mill., «klar for test» | Målemetode endres; ikke styrebehandlet | [OF-013] |
| 2026-03-05 | Full profilering: 12,4 % duplikater | R1 bekreftet | [EM-072] |
| 2026-04-19 | Kontraktsmodell reist; besluttet 2.6. (44 dager) | R2 | [OF-011] |
| 2026-05-11 | Linjen trekker tilbake 7 ressurser | R4 til forsinkelse | [EM-141] |
| 2026-06-13 | Migreringsverktøy levert, feiler | Leverandørforsinkelse | [EM-056] |
| 2026-06-17 | Bottoms-up 438 mill. | Gapet kjent internt | [EM-167, FIN-003] |
| 2026-07-02 | Bølge 1 redusert til 42 kunder | Skjult i hovedbildet | [EM-085, OF-007] |
| 2026-07-21 | Dobbelttelling på 40 mill. avdekket | Business case svekket | [EM-177] |
| 2026-08-26 | Styret får 395 og gul status; vedtak om samlet bilde | Styret har ikke full informasjon | [BOARD-005, BOARD-004] |
| 2026-09-10 | Reset utsatt til 22.9. | Beslutning ikke tatt | [OF-014] |
| 2026-09-16 | Kontrollert prognose 472 (455–494) | Gjeldende tall | [EM-173, FIN-005] |

Gjeldende versjoner: FIN-005 og EM-173 (16.9.) erstatter bottoms-up 438 [FIN-003] og base 459 [FIN-004]. BOARD-004 (26.8., ENDELIG) er siste styrepakke; 395 der er forbigått av 472.

## Motstridende forklaringer

> [!konflikt] Motstrid
> [EM-066] (Nordflow, kontraktsansvarlig) hevder leverandørsvikt er hoveddriver, mens [VEN-002] (Convergent, Aug 2026) hevder 10 av 18 integrasjoner skyldes Nordflow-beslutninger og data, 5 leverandørfeil, 3 delt. Uavklart per 2026-10-22. [TECH-005] (intern, 9.9.) gir 5/10/3, som støtter VEN-002; begge parter har egeninteresse i kreditt.

> [!konflikt] Motstrid
> [EM-104, EM-105] (9.–10.9.) oppgir 6 leverandørfeil av 18, mens [TECH-005] og [VEN-002] oppgir 5. Uavklart per 2026-10-22. Antall har variert mellom opptellinger (21 i juni, 19 i august [EM-099, EM-102]).

> [!konflikt] Motstrid
> [EM-053, EM-055, OF-010] hevder verktøyet var fem uker sent (ca. 6.5.), mens [EM-056] (nyere) sier det kom 13.6., om lag ti uker etter fristen 31.3. [EM-052]. Uavklart per 2026-10-22. Muligens ulike versjoner av verktøyet.

> [!konflikt] Motstrid
> [BOARD-004, OF-007] (26.8., ledelsesversjoner) hevder gul status og «håndterbar» kundesituasjon, mens [OF-008] (14.9., PMO-utkast) foreslår rød og [EM-008, EM-011] holdt data/migrering rød. [OPS-001, OF-010] viser fallende KPI-er og rød kunderisiko. Uavklart per 2026-10-22. Primærdata og PMO veier tyngre; Håkon Berg instruerte gul [EM-010].

> [!konflikt] Motstrid
> [BOARD-003] og [EM-199] forklarer saktere fart med endringsmotstand og energi, mens [HR-003], [EM-197] og [EM-125] sier dette ikke er hovedforklaring (skiftende prioriteringer, dobbeltansvar). Uavklart per 2026-10-22. HR-003 sier selv at målingen ikke fastslår motivasjon som primærårsak.

> [!konflikt] Motstrid
> [BOARD-003] (juni) oppgir gevinst 184 mill. fra 2028, mens [FIN-006] og [EM-178] (nyere) oppgir 128 mill. fra 2029. Uavklart per 2026-10-22. Primærregnearket og kildekontroll taler for 128.

> [!konflikt] Motstrid
> [EM-147] navngir de fem fornyelsene (Fjordkraft Drift, ScanMarine, MedicoLog, Vestbygg, Arctiq), mens [OPS-004] (12.9.) navngir EnergiVest, Nordbygg, Skandia, Metrohandel og Svea. Begge summerer til 146 mill. [EM-146]. Uavklart per 2026-10-22; OPS-004 er regneark og nyere.

> [!konflikt] Motstrid
> [VEN-002] sier Convergent er åpen for kreditt på 24–34 mill. ved scope-frys, mens [EM-067] (13.9.) avviser 34 mill. uten vurdering av 31 kundeskapte hendelser. Uavklart per 2026-10-22; kreditten er «ikke avtalt» [FIN-004] men ligger i prognosen [FIN-005].

Egeninteresse: Håkon Berg (programdirektør) vil ha gul og 395 [EM-010, EM-168]; Thomas Vik (CFO) skrev business casen, leder styringsgruppen og ville vente med nytt tall før bankmøtet [BOARD-001, EM-182]; Convergent og kontraktsansvarlig Ole Martin Kvale forhandler kreditt [EM-066].

## Kildekvalitet

| Kilde | Type og vekt | Merknad |
|---|---|---|
| BOARD-001/002, OF-001/002 | Primær (vedtak, mandat, plan); høy | CFO er forfatter av saken |
| OF-011, OF-010, OF-009 | Primærdata (beslutningslogg, risikoregister); høy | Udaterte; datoer i tillegg til EM-025/EM-030 stemmer ikke helt |
| TECH-004, TECH-005, HR-002, OPS-001, OPS-005 | Primærdata; høy | HR-002 er øyeblikksbilde, ikke snitt [EM-130] |
| FIN-003, FIN-005, FIN-007 | Regneark, kontrollert av Finance; høy | Brutto/netto og 395-broen går ikke opp (se hull) |
| BOARD-003/004, OF-006/007 | Ledelsesoppsummering; lav til middels | Selektive, bestilt av programdirektør [EM-010, EM-013] |
| TECH-002 | Utkast, CIO; middels | CIO anbefaler reset |
| VEN-002 | Leverandørposisjon; lav til middels | Egeninteresse; selv erkjenner den ikke er årsaksfordeling |
| EM-xxx | Påstander; varierer | Kvalitet følger avsender og rolle |
| EM-202–240 m.fl., OTHER-001 | Støy (kontor, ESG, Aurora) | Ikke brukt som årsaksbelegg |

## Usikkerhet og hull

- Vekting mellom R1–R4 er ikke målt. Det finnes ingen kritisk-sti-analyse som tallfester hver årsaks andel av forsinkelsen; ville kreve planfiler med avhengigheter.
- Hva som skjedde 22.9. (reset) og etter 17.9. finnes ikke i materialet.
- 395-broen går ikke opp: 395 pluss postene 41, 22, 19 og 29 gir 506, som er bruttotallet, mens 395 skal inkludere kreditt [EM-173, BOARD-003, FIN-005]. Uavklart om 395 er brutto eller netto; kilden til tidligere 382 er ikke funnet [EM-166].
- Dato-avvik: OF-011 sier kontraktsmodell reist 19.4., EM-027 sier 9.5.; median 35,5 sitert 22.8. [EM-030] stemmer med OF-011 først rundt 12.9.
- Planlagt FTE ved godkjenning og styrets faktiske rapportering (kvartalsvis) er ikke dokumentert; kun to styrepakker finnes.
- Andel av SLA-fallet og churn som skyldes OneFlow er ikke isolert [OPS-002].
- Leverandørens e-postdomene (synervia) avviker fra navnet Convergent; ikke avklart.

## Nøkkelkilder

- [BOARD-002]: styrets krav om porter og avstemming (kontrastér med utfallet).
- [OF-001] og [OF-002]: mandat og plan med manglende eierskap og status ved godkjenning.
- [OF-013]: hvordan recovery og målemetode ble vedtatt, og avgrensningen mot styret.
- [OF-011]: beslutningskøen i tall.
- [TECH-005] og [TECH-004]: årsaker til de 18 integrasjonene og datakvalitet.
- [VEN-002] og [VEN-001]: leverandørens syn og kontraktens ansvarsdeling.
- [FIN-003], [FIN-005] og [FIN-006]: kostnadsbro og gevinstkorrigering.
- [HR-002] og [HR-003]: kapasitet og belastning.
- [OPS-001] og [OPS-003]: kundevirkning og pilot.
- [EM-043] og [EM-145]: scope-vekst og effekten av ressurstrekk.

## Bidrag til leveranser

- **CEO-brief:** Si rett ut at kostnadsrommet er 455–494 mill. (base 472), ikke 395, og at årsaken er styring, forutsetninger og scope, ikke først og fremst leverandør eller motivasjon [FIN-005, TECH-005, HR-003].
- **Lederpresentasjon:** Vis årsak-virkning (R1–R4 til symptomer) og de ledelsesvalgene som forsterket, med konflikt om leverandøransvar vist åpent [VEN-002, EM-066].
- **90-dagersplan:** Tiltak må treffe årsakene: beslutningsforum med 7-dagers frist og navngitt eier (R2), eier for kunde-/inntektsrisiko, skjermet og finansiert kapasitet (R4), scope-frys med unntaksprosess (R3), porter for data og prosess (R1) [OF-014, OF-012, EM-050].
- **Evidenslogg:** Før R1–R4 som antakelser med belegg og falsifiseringstest, og legg inn konfliktblokkene og hullene over.
- **Styrekommunikasjon:** Styret har bedt om originalplan og recovery side om side og umiddelbar varsling av vesentlige endringer [BOARD-005]; dette må følges.
