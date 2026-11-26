# Dovolenkovač – Testovacie prípady: Výpočet dovolenkového nároku

**Projekt:** Dovolenkovač  
**Testovaná oblasť:** SP09 – Výpočet dovolenkového nároku  
**Typ testovania:** Manuálne funkčné testovanie

## Prehľad testovacích prípadov

| ID | Testovací prípad | Očakávaný výsledok | Výsledok |
|---|---|---|---|
| TC-010 | Výpočet počtu dní dovolenky podľa veku používateľa | Systém pridelí správny počet dní dovolenky podľa veku | Passed |
| TC-011 | Odpočítanie dní dovolenky po vytvorení žiadosti | Systém správne odpočíta dni dovolenky zo zostatku | Passed |

## TC-010 – Výpočet počtu dní dovolenky podľa veku používateľa

**Predpoklad:** Používateľ sa nachádza na registračnej stránke aplikácie.

**Kroky:**
1. Zaregistrovať používateľa s rokom narodenia 1979.
2. Dokončiť registráciu.
3. Skontrolovať počet dní dovolenky zobrazený v aplikácii.
4. Zopakovať test s rokom narodenia 2000.

**Očakávaný výsledok:**
- Používateľ narodený v roku 1979 (vek 46 rokov) má nárok na 25 dní dovolenky.
- Používateľ narodený v roku 2000 (vek 26 rokov) má nárok na 20 dní dovolenky.

**Skutočný výsledok:**
- Pri roku narodenia 1979 systém zobrazil 25 dní dovolenky.
- Pri roku narodenia 2000 systém zobrazil 20 dní dovolenky.

**Status:** Passed

## TC-011 – Odpočítanie dní dovolenky po vytvorení žiadosti

**Predpoklad:** Používateľ je prihlásený v aplikácii a má k dispozícii zostatok dní dovolenky.

**Kroky:**
1. Na úvodnej stránke Welcome kliknúť na tlačidlo Pokračovať.
2. Vybrať možnosť Nová žiadosť.
3. Zvoliť dátum začiatku a konca dovolenky.
4. Zadať žiadosť o dovolenku.
5. Skontrolovať aktualizovaný zostatok dní dovolenky.

**Očakávaný výsledok:** Systém zaregistruje žiadosť o dovolenku a odpočíta príslušný počet dní zo zostatku používateľa.

**Skutočný výsledok:** Systém zaregistroval žiadosť o dovolenku a správne odpočítal príslušný počet dní zo zostatku.

**Status:** Passed
