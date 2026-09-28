# Zhouyi Chart and Bazi Source Code | JavaScript Chinese Metaphysics

[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md) | [Product site](https://deeptexas-ai.github.io/Zhouyi-Bagua-Divination-Source-Code/)

This repository contains browser-oriented JavaScript source components for Chinese metaphysics chart generation. The public tree covers Four Pillars Bazi, stem-branch and lunar-calendar conversion, Ten Gods and Shen Sha, branch relationships, Five Elements, luck cycles, time zones and apparent solar-time inputs. Product screens and code also expose Qizheng Siyu, Da Liuren and API-driven Ziwei chart components.

> Scope: this page separates code-verified behavior from screenshot-demonstrated interfaces. The repository does not contain `package.json`, Docker configuration, a Python service, SQLite data or a complete 64-hexagram dataset. It should not be described as verified one-click deployment or a complete three-coin I Ching engine. Some UI flows call `/api` and require matching services.

## Product screens

| Bazi and luck cycles | Qizheng Siyu chart |
| --- | --- |
| ![Four Pillars Bazi luck cycles and solar time screen](docs/assets/screenshots/wujibazi.png) | ![Qizheng Siyu planets timezone and coordinates screen](docs/assets/screenshots/qizhengsiyu.png) |
| Da Liuren chart | Five Elements trend and history |
| ![Da Liuren chart result with Heaven and Earth plates](docs/assets/screenshots/daliuren.png) | ![Five Elements trend chart and saved chart history](docs/assets/screenshots/wuxing.png) |

## Verified capabilities

### Four Pillars and calendar calculations

- Generate stems, branches, pillars and related Ten Gods data from date and time.
- Convert solar and lunar calendars with terms, zodiac and Julian-day components.
- Display major luck cycles and annual, monthly, daily and hourly periods.
- Accept timezone, coordinates and apparent solar-time related inputs.

### Five Elements, Ten Gods and Shen Sha

- Map stems and branches to Wood, Fire, Earth, Metal and Water.
- Represent hidden stems and clash, combination, harm and punishment relationships.
- Query Shen Sha rules and descriptions implemented in `shensha.js`.
- Render Five Elements parameters, trends and chart-history interfaces.

### Qizheng Siyu, Da Liuren and extension components

- Qizheng Siyu planet selection, coordinates, timezone and result interfaces.
- Da Liuren calculation components in `kinliuren.js`.
- Ziwei trend and reverse-query API calls plus chart rendering in `index.js`.
- Search-chart, palace, Nine Stars and Eight Gates filters visible in product screens.

## Source map

| File | Verified responsibility |
| --- | --- |
| `index.html` / `index.js` | Chart UI, input flows, visualization and API interaction |
| `lunar.js` / `nongli.js` | Solar/lunar calendar, stems, branches and solar terms |
| `paipan.js` | Astronomical calendar, solar terms, apparent solar time and luck cycles |
| `paipan.gx.js` | Ten Gods, hidden stems and stem/branch relationships |
| `shensha.js` | Shen Sha rules, descriptions and lookup |
| `kinliuren.js` | Da Liuren calculations |
| `timezone.js` | Timezone, coordinate and offset data |

## More real screenshots

| Chart search filters | Annual planet positions |
| --- | --- |
| ![Bazi chart search conditions and pattern filters](docs/assets/screenshots/baizhipaipan.png) | ![Annual planet longitude and chart data](docs/assets/screenshots/liunian.png) |
| Qizheng Siyu result | Planet combination output |
| ![Qizheng Siyu detailed chart table](docs/assets/screenshots/paipan.png) | ![Qizheng Siyu multi-column planet output](docs/assets/screenshots/qizheng2.png) |

## Runtime and responsible-use boundary

The public files can be inspected directly, but the complete runtime may depend on styles, chart libraries and `/api` services outside this tree. Verify dependencies, licenses, service implementations, privacy and calculation results before deployment. Divination content is for cultural study and entertainment and must not replace medical, legal, investment or other professional advice.

## Contact

- Telegram: [@xuzongbin001](https://t.me/xuzongbin001)
- Email: [masterai918@gmail.com](mailto:masterai918@gmail.com)

## License

See [License.md](License.md). Third-party calendar and algorithm code may retain separate attribution and license requirements; verify each component before commercial use.
