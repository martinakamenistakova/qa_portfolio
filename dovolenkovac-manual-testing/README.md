# Dovolenkovač – Manuálne testovanie webovej aplikácie

## O projekte

Dovolenkovač je webová aplikácia určená na správu dovoleniek zamestnancov. Projekt bol súčasťou praktickej skupinovej úlohy v rámci vzdelávacieho programu Women Tester Academy (Aj Ty v IT).

Cieľom projektu bolo analyzovať požiadavky, pripraviť testovacie prípady, vykonať manuálne testovanie aplikácie a zdokumentovať zistené chyby.

**Moja úloha v projekte**

V rámci skupinového projektu som zodpovedala za dve oblasti:

- TP3.1 – Registrácia: testovanie registračného procesu, validácie vstupných údajov a správania aplikácie po registrácii.

- SP09 – Výpočet dovolenkového nároku: overenie výpočtu počtu dní dovolenky podľa veku používateľa a správneho odpočítania dní po vytvorení žiadosti o dovolenku.

Pridelené oblasti som spracovala prevažne samostatne.

## Rozsah testovania a výsledky

V rámci pridelených oblastí som vytvorila a vykonala celkovo 11 testovacích prípadov.

7 testovacích prípadov bolo úspešných.

4 testovacie prípady skončili neúspešne a viedli k identifikácii chýb v registračnom procese.

## Použité nástroje a dokumentácia

- **JIRA** – evidencia a správa nájdených chýb.

- **Manuálne testovanie** – vykonávanie testovacích prípadov a overovanie funkčnosti aplikácie.

- **Markdown** – dokumentácia testovacích prípadov a bug reportov.

## Dokumentácia

**Testovacie prípady**

- [TP3.1 – Registrácia](test_cases/registracia.md)

- [SP09 – Výpočet dovolenkového nároku](test_cases/dovolenkovy_narok.md)

**Bug reporty**

- [**WTA24-47** – Registrácia s neplatným rokom narodenia](bug_reports/WTA24-47-neplatny-rok-narodenia.md)

- [**WTA24-48** – Chýbajúca e-mailová notifikácia po registrácii](bug_reports/WTA24-48-chybajuca-emailova-notifikacia.md)

- [**WTA24-49** – Chýbajúce potvrdenie úspešnej registrácie](bug_reports/WTA24-49-chybajuce-potvrdenie-registracie.md)

- [**WTA24-50** – Automatické prihlásenie po registrácii](bug_reports/WTA24-50-automaticke-prihlasenie.md)

*Projekt bol realizovaný v rámci Women Tester Academy – Aj Ty v IT.*
