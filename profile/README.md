# VilémIS

**Opensource CRM a systém pro správu projektů**

Česká open-source alternativa k velkým CRM platformám — postavená na React frontendu a PHP backendu s důrazem na jednoduchost a přizpůsobitelnost.

## Co VilémIS umí

- **Klienti & projekty** — správa kontaktů, firem a projektů na jednom místě
- **Úkoly & čas** — sledování úkolů, časové záznamy, opakující se úkoly
- **Faktury & nabídky** — tvorba faktur, nabídek a sledování plateb
- **E-mail** — integrovaná emailová schránka s pravidly a šablonami
- **Know-how** — interní wiki pro sdílení znalostí týmu
- **Vlastní entity** — flexibilní tvorba vlastních datových typů
- **Dashboard** — přehledový panel s grafy a statistikami

## Technologie

| Vrstva | Technologie |
|--------|------------|
| Frontend | React 19, React Router 7, Bootstrap 5, Material UI |
| Backend | PHP 8+, Gephart Framework, JWT |
| Databáze | MariaDB 10.11 |
| Infrastruktura | Docker, Redis |

## Začít je snadné

```bash
git clone https://github.com/vilemis/vilemis.git
cd vilemis
cp api/v1/config/orm.json--default api/v1/config/orm.json
cp api/v1/config/security.json--default api/v1/config/security.json
docker-compose up && npm install && npm start
```

## Přispívání

Příspěvky jsou vítány! Viz [CONTRIBUTING](https://github.com/vilemis/vilemis#přispívání) v hlavním repozitáři.

---

[![Frontend Tests](https://github.com/vilemis/vilemis/actions/workflows/frontend-tests.yml/badge.svg)](https://github.com/vilemis/vilemis/actions/workflows/frontend-tests.yml)
[![PHP Tests](https://github.com/vilemis/vilemis/actions/workflows/php.yml/badge.svg)](https://github.com/vilemis/vilemis/actions/workflows/php.yml)
[![Licence: MIT](https://img.shields.io/badge/Licence-MIT-yellow.svg)](https://github.com/vilemis/vilemis/blob/main/LICENSE)
