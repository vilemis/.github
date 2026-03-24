# VilémIS

**CRM pro freelancery — open source, bez předplatného**

Spravujte klienty, projekty, faktury a čas na jednom místě. Žádné měsíční poplatky, žádný vendor lock-in — prostě nainstalujte a používejte.

## Pro koho je VilémIS?

Pro **freelancery**, kteří potřebují mít přehled o svých klientech, projektech a financích — bez zbytečně složitých systémů a bez placení za každého uživatele.

## Co řeší

| Problém freelancera | Řešení v VilémIS |
|---------------------|-----------------|
| Kde mám ty hodiny od klienta? | Časové záznamy per projekt/úkol |
| Faktura za tento měsíc? | Generování faktur z odpracovaného času |
| Co jsme s klientem řešili? | Historie emailů, komentářů a aktivit |
| Kde je ta smlouva / přihlašovací údaje? | Přílohy a šifrovaný heslovník u klienta |
| Neztratit se v desítkách klientů najednou | Přehledný dashboard s financemi a aktivitami |

## Rychlý start

```bash
git clone https://github.com/vilemis/vilemis.git
cd vilemis
cp api/v1/config/orm.json--default api/v1/config/orm.json
cp api/v1/config/security.json--default api/v1/config/security.json
docker-compose up && npm install && npm start
```

Systém běží na `http://localhost:3000`. Databáze, backend i Redis se spustí automaticky přes Docker.

## Funkce

- Klienti, kontakty, projekty, úkoly
- Sledování času a opakující se úkoly
- Faktury, nabídky, náklady
- Integrovaná emailová schránka (IMAP/SMTP)
- Šifrovaný heslovník pro přihlašovací údaje klientů
- Vlastní datové typy (custom entities)
- Dashboard s přehledem financí a aktivit

## Technologie

React 19 · PHP 8+ · MariaDB 10.11 · Docker · MIT licence

---

[![Frontend Tests](https://github.com/vilemis/vilemis/actions/workflows/frontend-tests.yml/badge.svg)](https://github.com/vilemis/vilemis/actions/workflows/frontend-tests.yml)
[![PHP Tests](https://github.com/vilemis/vilemis/actions/workflows/php.yml/badge.svg)](https://github.com/vilemis/vilemis/actions/workflows/php.yml)
[![Licence: MIT](https://img.shields.io/badge/Licence-MIT-yellow.svg)](https://github.com/vilemis/vilemis/blob/main/LICENSE)
