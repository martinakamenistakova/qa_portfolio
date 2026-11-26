# WTA24-48 – Chýbajúca e-mailová notifikácia po registrácii

**Projekt:** Dovolenkovač  
**Typ:** Bug  
**Pôvodné JIRA ID:** WTA24-48  
**Pôvodná priorita:** Minor  
**Oblasť:** Registrácia  
**Test case:** TC-007  
**Prostredie:** TEST, Google Chrome 149.0.7827.200, Windows 11

## Popis chyby

Po úspešnej registrácii aplikácia neodošle používateľovi e-mailovú notifikáciu o registrácii.

## Kroky na reprodukciu

1. Otvoriť stránku Registrácia.
2. Vyplniť všetky povinné polia platnými údajmi vrátane e-mailovej adresy.
3. Stlačiť tlačidlo Registrovať.
4. Skontrolovať e-mailovú schránku zadanú pri registrácii.

## Očakávaný výsledok

Aplikácia odošle na zadanú e-mailovú adresu notifikáciu o úspešnej registrácii.

## Skutočný výsledok

Do zadanej e-mailovej schránky nebola doručená žiadna notifikácia o registrácii.
