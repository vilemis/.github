# VilémIS

**CRM pro freelancery a malé agentury — open source, bez předplatného**

Spravujte klienty, projekty, faktury a čas na jednom místě. Žádné měsíční poplatky, žádný vendor lock-in — prostě nainstalujte a používejte.

## Pro koho je VilémIS?

- **Freelancery** — fakturace, sledování hodin, přehled klientů a projektů
- **Malé agentury** — sdílení projektů v týmu, správa úkolů, know-how wiki
- **Vývojáře** — snadné rozšíření, vlastní entity, Docker setup za 5 minut

## Co řeší

| Problém | Řešení v VilémIS |
|---------|-----------------|
| Kde mám ty hodiny od klienta? | Časové záznamy per projekt/úkol |
| Faktura za tento měsíc? | Generování faktur z odpracovaného času |
| Co jsme s klientem řešili? | Historie emailů, komentářů a aktivit |
| Kde je ta smlouva? | Přílohy a dokumenty u klienta/projektu |
| Jak sdílet know-how v týmu? | Interní wiki přímo v systému |

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
- Vlastní datové typy (custom entities)
- Dashboard s přehledem financí a aktivit
- Heslovník (šifrovaný) pro přihlašovací údaje klientů

## Technologie

React 19 · PHP 8+ · MariaDB 10.11 · Docker · MIT licence

---

[![Frontend Tests](https://github.com/vilemis/vilemis/actions/workflows/frontend-tests.yml/badge.svg)](https://github.com/vilemis/vilemis/actions/workflows/frontend-tests.yml)
[![PHP Tests](https://github.com/vilemis/vilemis/actions/workflows/php.yml/badge.svg)](https://github.com/vilemis/vilemis/actions/workflows/php.yml)
[![Licence: MIT](https://img.shields.io/badge/Licence-MIT-yellow.svg)](https://github.com/vilemis/vilemis/blob/main/LICENSE)
