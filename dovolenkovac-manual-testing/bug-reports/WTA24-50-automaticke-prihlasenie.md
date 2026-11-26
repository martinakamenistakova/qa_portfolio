WTA24-50 – Automatické prihlásenie po registrácii

**Projekt:** Dovolenkovač  
**Typ:** Bug  
**Pôvodné JIRA ID:** WTA24-50  
**Pôvodná priorita:** Minor  
**Oblasť:** Registrácia  
**Test case:** TC-009  
**Prostredie:** TEST, Google Chrome 149.0.7827.200, Windows 11

## Popis chyby

Po úspešnej registrácii aplikácia používateľa automaticky prihlási namiesto presmerovania na prihlasovaciu stránku.

## Kroky na reprodukciu

1. Otvoriť stránku Registrácia.
2. Vyplniť všetky povinné polia platnými údajmi.
3. Stlačiť tlačidlo Registrovať.

## Očakávaný výsledok

Aplikácia zobrazí stránku Prihlásenie.

## Skutočný výsledok

Aplikácia používateľa automaticky prihlási do jeho konta.
