# WTA24-47 – Registrácia s neplatným rokom narodenia

**Projekt:** Dovolenkovač  
**Typ:** Bug  
**Pôvodné JIRA ID:** WTA24-47  
**Pôvodná priorita:** Minor  
**Oblasť:** Registrácia  
**Test case:** TC-003  
**Prostredie:** TEST, Google Chrome 149.0.7827.200, Windows 11

## Popis chyby

Aplikácia umožňuje registráciu používateľa aj pri zadaní neplatného roku narodenia.

## Kroky na reprodukciu

1. Otvoriť stránku Registrácia.
2. Do poľa Dátum narodenia zadať rok 1890.
3. Stlačiť tlačidlo Registrovať.

## Očakávaný výsledok

Aplikácia zobrazí upozornenie na neplatný rok narodenia a neumožní dokončiť registráciu.

## Skutočný výsledok
