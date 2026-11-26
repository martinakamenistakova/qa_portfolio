# Dovolenkovač – Testovacie prípady: Registrácia

**Projekt:** Dovolenkovač  
**Testovaná oblasť:** TP3.1 – Registrácia  
**Typ testovania:** Manuálne funkčné testovanie

## Prehľad testovacích prípadov

| ID | Testovací prípad | Očakávaný výsledok | Výsledok |
|---|---|---|---|
| TC-001 | Registrácia s prázdnymi povinnými poľami | Systém označí povinné polia | Passed |
| TC-002 | Registrácia s neplatným formátom e-mailu | Systém upozorní na neplatný formát e-mailu | Passed |
| TC-003 | Registrácia s neplatným rokom narodenia | Systém neumožní registráciu | Failed |
| TC-004 | Registrácia s už existujúcou e-mailovou adresou | Systém upozorní na duplicitný e-mail | Passed |
| TC-005 | Registrácia s rozdielnym heslom a potvrdením hesla | Systém upozorní na nezhodu hesiel | Passed |
| TC-006 | Opakovaná registrácia s rovnakými údajmi | Systém upozorní na existujúce údaje | Passed |
| TC-007 | E-mailová notifikácia po registrácii | Používateľ dostane e-mailovú notifikáciu | Failed |
| TC-008 | Potvrdenie úspešnej registrácie | Systém zobrazí potvrdenie registrácie | Failed |
| TC-009 | Správanie systému po úspešnej registrácii | Systém zobrazí prihlasovaciu stránku | Failed |

## TC-001 – Registrácia s prázdnymi povinnými poľami

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia.

**Kroky:**
1. Otvoriť stránku Registrácia.
2. Pokúsiť sa pokračovať bez vyplnenia povinných polí.
3. Postupne vypĺňať jednotlivé povinné polia.

**Očakávaný výsledok:** Systém označí povinné polia, ktoré je potrebné vyplniť.

**Skutočný výsledok:** Systém označuje povinné polia postupne po vyplnení predchádzajúcich polí.

**Status:** Passed

## TC-002 – Registrácia s neplatným formátom e-mailu

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia.

**Kroky:**
1. Vyplniť registračný formulár.
2. Do poľa E-mail zadať adresu bez znaku `@`.
3. Pokúsiť sa dokončiť registráciu.

**Očakávaný výsledok:** Systém upozorní používateľa na neplatný formát e-mailovej adresy.

**Skutočný výsledok:** Systém zobrazí upozornenie na neplatný formát e-mailovej adresy.

**Status:** Passed

## TC-003 – Registrácia s neplatným rokom narodenia

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia.

**Kroky:**
1. Vyplniť registračný formulár platnými údajmi.
2. Do poľa Dátum narodenia zadať rok 1890.
3. Stlačiť tlačidlo Registrovať.

**Očakávaný výsledok:** Systém upozorní na neplatný rok narodenia a neumožní dokončiť registráciu.

**Skutočný výsledok:** Systém umožní registráciu aj napriek neplatnému roku narodenia.

**Status:** Failed

**Poznámka:** Rovnaké správanie bolo pozorované aj pri zadaní budúceho roku narodenia 2050.

**Súvisiaci bug report:** WTA24-47

## TC-004 – Registrácia s už existujúcou e-mailovou adresou

**Predpoklad:** V systéme už existuje používateľ s danou e-mailovou adresou.

**Kroky:**
1. Otvoriť stránku Registrácia.
2. Vyplniť registračný formulár.
3. Použiť e-mailovú adresu, ktorá už bola zaregistrovaná.
4. Pokúsiť sa dokončiť registráciu.

**Očakávaný výsledok:** Systém upozorní používateľa, že e-mailová adresa už existuje.

**Skutočný výsledok:** Systém zobrazí upozornenie na duplicitnú e-mailovú adresu.

**Status:** Passed

## TC-005 – Registrácia s rozdielnym heslom a potvrdením hesla

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia.

**Kroky:**
1. Vyplniť registračný formulár.
2. Do poľa Heslo zadať heslo.
3. Do poľa Potvrdenie hesla zadať odlišné heslo.
4. Pokúsiť sa dokončiť registráciu.

**Očakávaný výsledok:** Systém upozorní používateľa na nezhodu hesiel a neumožní dokončiť registráciu.

**Skutočný výsledok:** Systém zobrazí upozornenie na nezhodu hesiel.

**Status:** Passed

## TC-006 – Opakovaná registrácia s rovnakými údajmi

**Predpoklad:** Používateľ už úspešne dokončil registráciu s danými údajmi.

**Kroky:**
1. Otvoriť stránku Registrácia.
2. Opätovne vyplniť formulár rovnakými údajmi ako pri predchádzajúcej registrácii.
3. Pokúsiť sa dokončiť registráciu.

**Očakávaný výsledok:** Systém rozpozná existujúce údaje a upozorní používateľa na duplicitu.

**Skutočný výsledok:** Systém zobrazí upozornenie na duplicitné údaje.

**Status:** Passed

## TC-007 – E-mailová notifikácia po registrácii

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia a má k dispozícii funkčnú e-mailovú schránku.

**Kroky:**
1. Vyplniť všetky povinné polia platnými údajmi vrátane e-mailovej adresy.
2. Stlačiť tlačidlo Registrovať.
3. Skontrolovať e-mailovú schránku zadanú pri registrácii.

**Očakávaný výsledok:** Používateľ dostane e-mailovú notifikáciu o úspešnej registrácii.

**Skutočný výsledok:** Do zadanej e-mailovej schránky nebola doručená žiadna notifikácia o registrácii.

**Status:** Failed

**Súvisiaci bug report:** WTA24-48

## TC-008 – Potvrdenie úspešnej registrácie

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia.

**Kroky:**
1. Vyplniť všetky povinné polia platnými údajmi.
2. Stlačiť tlačidlo Registrovať.

**Očakávaný výsledok:** Systém zobrazí informáciu potvrdzujúcu úspešnú registráciu používateľa.

**Skutočný výsledok:** Systém nezobrazí žiadnu informáciu o úspešnej registrácii.

**Status:** Failed

**Súvisiaci bug report:** WTA24-49

## TC-009 – Správanie systému po úspešnej registrácii

**Predpoklad:** Používateľ sa nachádza na stránke Registrácia.

**Kroky:**
1. Vyplniť všetky povinné polia platnými údajmi.
2. Stlačiť tlačidlo Registrovať.

**Očakávaný výsledok:** Systém zobrazí stránku Prihlásenie.

**Skutočný výsledok:** Systém používateľa automaticky prihlási do jeho konta.

**Status:** Failed

**Súvisiaci bug report:** WTA24-50
