# Game Translator

> 🇺🇸 Auto-translate **Ren'Py visual novels** to your language. Free, no API key, no Python needed.
> 🇧🇷 Traduza **visual novels Ren'Py** para o seu idioma automaticamente. Grátis, sem chave de API.
> 🇪🇸 Traduce **visual novels Ren'Py** a tu idioma automáticamente. Gratis, sin clave API.
> 🇷🇺 Автоматический перевод **визуальных новелл Ren'Py** на ваш язык. Бесплатно, без API ключа.

[![Latest Release](https://img.shields.io/github/v/release/A2Reis/renpy-translator?style=flat-square)](https://github.com/A2Reis/renpy-translator/releases/latest)
[![License](https://img.shields.io/badge/license-Proprietary-blue?style=flat-square)](#license)
[![Windows](https://img.shields.io/badge/Windows-10%2F11-0078d4?style=flat-square&logo=windows)](#download)

**[Download latest release →](https://github.com/A2Reis/renpy-translator/releases/latest)**

---

<details open>
<summary><h2>🇺🇸 English</h2></summary>

### Why Game Translator?

Translate any **Ren'Py visual novel** to **133+ languages** with a single click. No script editing, no API keys, no monthly fees.

| | **Game Translator** | translator++ | Online OCR | Manual |
|---|---|---|---|---|
| Free | ✅ | ✅ | ⚠️ Limited | ✅ |
| No API key | ✅ | ❌ | ❌ | ✅ |
| Offline after first scan | ✅ Local cache | ❌ | ❌ | ✅ |
| Translates **before** playing | ✅ Pre-scan | ⚠️ Per-line | ❌ Real-time | ✅ |
| Preserves variables `[Name]` | ✅ | ⚠️ Fragile | ❌ | ⚠️ |
| Auto-handles `.rpa` archives | ✅ | ❌ | ❌ | ❌ |
| Quality validator | ✅ | ❌ | ❌ | N/A |
| Backup + 1-click restore | ✅ | ⚠️ Manual | N/A | ❌ |
| Portable `.exe`, no Python | ✅ ~57MB | ❌ | Browser | N/A |

### Quick Start

1. **[Download `GameTranslator.exe`](https://github.com/A2Reis/renpy-translator/releases/latest)** — no installation
2. Point to your game's `game/` folder (e.g., `Steam\steamapps\common\<Game>\game`)
3. Click **Iniciar Pre-scan** and wait 5-10 min (first time; later runs are seconds)
4. Open the game — fully translated. To revert: click **Restaurar Backup**

### Translation Quality

| Problem | How we handle it |
|---|---|
| `[player_name]` getting translated | Variables masked before sending to Google |
| Wrong sense for short words (`Fine.` → wrong verb) | Curated dict with 55+ dialogue overrides |
| Ambiguous pronouns in pt-BR ("pegar [Name]" = sexual) | Regex post-fix swaps to neutral verb |
| Names treated as verbs | Proper-name detector with stopword list |
| Save game compatibility | Inline writer preserves line numbers + Ren'Py IDs |
| Cache poisoned by old errors | 6 automated migrations clean entries on open |

Built-in **validator** scans translations for common issues (wrong names, length outliers, untranslated lines, wrong-language output) and offers one-click auto-fix.

### Supported Languages

Any of the **133+ languages** Google Translate supports. Production-tested for:

- 🇧🇷 Portuguese (Brazil) — 55+ curated dialogue overrides
- 🇪🇸 Spanish, 🇫🇷 French, 🇩🇪 German, 🇮🇹 Italian
- 🇯🇵 Japanese, 🇨🇳 Chinese, 🇰🇷 Korean
- 🇷🇺 Russian, 🇵🇱 Polish, 🇸🇪 Swedish, 🇳🇱 Dutch

### Supported Games

Any visual novel built with the **[Ren'Py engine](https://www.renpy.org/)**, including those distributed via:
- Steam
- itch.io
- Direct downloads / community forums

Works with games that ship with encrypted `.rpa` archives — extraction, decompilation, translation, and re-injection happen automatically.

**Experimental** support: RPG Maker MV/MZ, Godot.

### Requirements

- Windows 10/11 (64-bit) — official builds
- ~500 MB free disk space (cache + extracted scripts)
- Internet during first scan (cached afterwards)

### Privacy

- **No telemetry**, no analytics, no "phone home"
- **No account required** — runs entirely on your machine
- Translation requests go to **Google Translate** (the same public endpoint Chrome's "Translate this page" uses)
- All caches are local SQLite files in `%AppData%\GameTranslator\`
- Original game files are **backed up automatically** before any modification

</details>

---

<details>
<summary><h2>🇧🇷 Português (Brasil)</h2></summary>

### Por que usar?

Traduza qualquer **visual novel Ren'Py** para **mais de 133 idiomas** com um clique. Sem editar scripts, sem chave de API, sem mensalidade.

| | **Game Translator** | translator++ | OCR online | Manual |
|---|---|---|---|---|
| Grátis | ✅ | ✅ | ⚠️ Limitado | ✅ |
| Sem chave de API | ✅ | ❌ | ❌ | ✅ |
| Funciona offline após 1ª scan | ✅ Cache local | ❌ | ❌ | ✅ |
| Traduz **antes** de jogar | ✅ Pre-scan | ⚠️ Por linha | ❌ Tempo real | ✅ |
| Preserva variáveis `[Nome]` | ✅ | ⚠️ Frágil | ❌ | ⚠️ |
| Lida com arquivos `.rpa` | ✅ | ❌ | ❌ | ❌ |
| Validador de qualidade | ✅ | ❌ | ❌ | N/A |
| Backup + restauração 1 clique | ✅ | ⚠️ Manual | N/A | ❌ |
| `.exe` portátil, sem Python | ✅ ~57MB | ❌ | Browser | N/A |

### Início Rápido

1. **[Baixe `GameTranslator.exe`](https://github.com/A2Reis/renpy-translator/releases/latest)** — sem instalação
2. Aponte para a pasta `game/` do jogo (ex: `Steam\steamapps\common\<Jogo>\game`)
3. Clique **Iniciar Pre-scan** e espere 5-10 min (primeira vez; depois é segundos)
4. Abra o jogo — totalmente traduzido. Pra reverter: clique **Restaurar Backup**

### Qualidade de Tradução

| Problema | Como resolvemos |
|---|---|
| `[player_name]` sendo traduzido | Variáveis mascaradas antes de mandar pro Google |
| Sentido errado pra palavras curtas (`Fine.` → verbo errado) | Dict curado com 55+ overrides de diálogo |
| Pronomes ambíguos em pt-BR ("pegar [Nome]" = sexual) | Regex post-fix troca por verbo neutro |
| Nomes tratados como verbos | Detector de nome próprio com lista de stopwords |
| Compatibilidade de saves | Writer inline preserva números de linha + IDs do Ren'Py |
| Cache poluído por erros antigos | 6 migrations automáticas limpam entradas ruins na abertura |

**Validador** embutido analisa traduções em busca de erros (nomes errados, comprimento fora de padrão, linhas não traduzidas, saída em idioma errado) e oferece correção automática em 1 clique.

### Idiomas Suportados

Qualquer um dos **133+ idiomas** do Google Translate. Testado em produção para:

- 🇧🇷 Português (Brasil) — 55+ overrides de diálogo curados
- 🇪🇸 Espanhol, 🇫🇷 Francês, 🇩🇪 Alemão, 🇮🇹 Italiano
- 🇯🇵 Japonês, 🇨🇳 Chinês, 🇰🇷 Coreano
- 🇷🇺 Russo, 🇵🇱 Polonês, 🇸🇪 Sueco, 🇳🇱 Holandês

### Jogos Suportados

Qualquer visual novel feita com a **[engine Ren'Py](https://www.renpy.org/)**, incluindo distribuídos via:
- Steam
- itch.io
- Downloads diretos / fóruns da comunidade

Funciona com jogos que vêm com arquivos `.rpa` encriptados — extração, decompilação, tradução e re-injeção acontecem automaticamente.

Suporte **experimental**: RPG Maker MV/MZ, Godot.

### Requisitos

- Windows 10/11 (64-bit) — builds oficiais
- ~500 MB de espaço em disco (cache + scripts extraídos)
- Internet durante a primeira scan (depois fica em cache)

### Privacidade

- **Sem telemetria**, sem analytics, sem "phone home"
- **Sem conta necessária** — roda 100% na sua máquina
- Requisições vão pro **Google Translate** (mesmo endpoint público que o "Traduzir esta página" do Chrome)
- Cache local em SQLite no `%AppData%\GameTranslator\`
- Arquivos originais do jogo são **backupeados automaticamente** antes de qualquer modificação

</details>

---

<details>
<summary><h2>🇪🇸 Español</h2></summary>

### ¿Por qué Game Translator?

Traduce cualquier **visual novel Ren'Py** a **más de 133 idiomas** con un clic. Sin editar scripts, sin claves API, sin suscripciones.

| | **Game Translator** | translator++ | OCR online | Manual |
|---|---|---|---|---|
| Gratis | ✅ | ✅ | ⚠️ Limitado | ✅ |
| Sin clave API | ✅ | ❌ | ❌ | ✅ |
| Offline tras primer escaneo | ✅ Caché local | ❌ | ❌ | ✅ |
| Traduce **antes** de jugar | ✅ Pre-scan | ⚠️ Por línea | ❌ Tiempo real | ✅ |
| Preserva variables `[Nombre]` | ✅ | ⚠️ Frágil | ❌ | ⚠️ |
| Maneja archivos `.rpa` | ✅ | ❌ | ❌ | ❌ |
| Validador de calidad | ✅ | ❌ | ❌ | N/A |
| Backup + restauración 1 clic | ✅ | ⚠️ Manual | N/A | ❌ |
| `.exe` portátil, sin Python | ✅ ~57MB | ❌ | Navegador | N/A |

### Inicio Rápido

1. **[Descarga `GameTranslator.exe`](https://github.com/A2Reis/renpy-translator/releases/latest)** — sin instalación
2. Apunta a la carpeta `game/` del juego (ej: `Steam\steamapps\common\<Juego>\game`)
3. Haz clic en **Iniciar Pre-scan** y espera 5-10 min (primera vez; después son segundos)
4. Abre el juego — completamente traducido. Para revertir: clic en **Restaurar Backup**

### Idiomas Soportados

Cualquiera de los **133+ idiomas** que admite Google Translate. Probado en producción para:

- 🇧🇷 Portugués (Brasil), 🇪🇸 Español, 🇫🇷 Francés, 🇩🇪 Alemán, 🇮🇹 Italiano
- 🇯🇵 Japonés, 🇨🇳 Chino, 🇰🇷 Coreano
- 🇷🇺 Ruso, 🇵🇱 Polaco, 🇸🇪 Sueco, 🇳🇱 Neerlandés

### Juegos Soportados

Cualquier visual novel hecha con el **[motor Ren'Py](https://www.renpy.org/)**, incluyendo los distribuidos por Steam, itch.io, descargas directas y foros de la comunidad.

Funciona con juegos que vienen con archivos `.rpa` encriptados — extracción, decompilación, traducción y reinyección son automáticas.

Soporte **experimental**: RPG Maker MV/MZ, Godot.

### Requisitos

- Windows 10/11 (64 bits)
- ~500 MB de espacio libre
- Internet durante el primer escaneo (después se usa caché)

### Privacidad

- **Sin telemetría**, sin analytics
- **Sin cuenta** — funciona 100% en tu máquina
- Solicitudes a **Google Translate** (mismo endpoint público que usa Chrome)
- Archivos originales del juego son **respaldados automáticamente**

</details>

---

<details>
<summary><h2>🇷🇺 Русский</h2></summary>

### Зачем Game Translator?

Переводите любую **визуальную новеллу Ren'Py** на **133+ языков** одним кликом. Без редактирования скриптов, без API ключей, без подписок.

| | **Game Translator** | translator++ | Онлайн OCR | Вручную |
|---|---|---|---|---|
| Бесплатно | ✅ | ✅ | ⚠️ Ограничено | ✅ |
| Без API ключа | ✅ | ❌ | ❌ | ✅ |
| Работает офлайн после первого сканирования | ✅ Локальный кэш | ❌ | ❌ | ✅ |
| Переводит **до** игры | ✅ Pre-scan | ⚠️ Построчно | ❌ Real-time | ✅ |
| Сохраняет переменные `[Имя]` | ✅ | ⚠️ Хрупко | ❌ | ⚠️ |
| Обрабатывает `.rpa` архивы | ✅ | ❌ | ❌ | ❌ |
| Встроенный валидатор качества | ✅ | ❌ | ❌ | N/A |
| Бэкап + восстановление в 1 клик | ✅ | ⚠️ Вручную | N/A | ❌ |
| Портативный `.exe`, без Python | ✅ ~57МБ | ❌ | Браузер | N/A |

### Быстрый Старт

1. **[Скачайте `GameTranslator.exe`](https://github.com/A2Reis/renpy-translator/releases/latest)** — без установки
2. Укажите папку `game/` игры (например, `Steam\steamapps\common\<Игра>\game`)
3. Нажмите **Iniciar Pre-scan** и подождите 5-10 минут (первый раз; потом — секунды)
4. Откройте игру — полностью переведена. Для отката: нажмите **Restaurar Backup**

### Поддерживаемые Языки

Любой из **133+ языков**, поддерживаемых Google Translate. Проверено в продакшене для:

- 🇧🇷 Португальский (Бразилия), 🇪🇸 Испанский, 🇫🇷 Французский, 🇩🇪 Немецкий, 🇮🇹 Итальянский
- 🇯🇵 Японский, 🇨🇳 Китайский, 🇰🇷 Корейский
- 🇷🇺 Русский, 🇵🇱 Польский, 🇸🇪 Шведский, 🇳🇱 Голландский

### Поддерживаемые Игры

Любая визуальная новелла, созданная на **[движке Ren'Py](https://www.renpy.org/)**, включая распространяемые через Steam, itch.io, прямые загрузки и форумы сообщества.

Работает с играми, которые поставляются с зашифрованными `.rpa` архивами — извлечение, декомпиляция, перевод и повторное внедрение происходят автоматически.

**Экспериментальная** поддержка: RPG Maker MV/MZ, Godot.

### Требования

- Windows 10/11 (64-bit)
- ~500 МБ свободного места
- Интернет во время первого сканирования (потом кэш)

### Конфиденциальность

- **Без телеметрии**, без аналитики
- **Без учётной записи** — работает полностью на вашем компьютере
- Запросы идут в **Google Translate** (тот же публичный endpoint, что Chrome использует для перевода страниц)
- Оригинальные файлы игры **автоматически бэкапятся** перед любыми изменениями

</details>

---

## 🐛 Troubleshooting / Suporte / Soporte / Поддержка

**My old saves crash after re-translating** — Ren'Py saves reference exact script positions. Re-translating shifts lines slightly. Use the game's **Skip** mode (Tab/Ctrl) to fast-forward.

**Some menu choices are still in English** — Run the pre-scan again with the latest version. Recent versions fixed parser bugs that missed certain menu choice patterns.

**Can't find the game** — Point to the `game/` folder *inside* the game's directory, not the parent. Look for the folder containing `script.rpy` or `script.rpyc`.

**Translation has errors** — Use the **Validar** tab to scan + auto-fix common issues.

Open an issue: [GitHub Issues](https://github.com/A2Reis/renpy-translator/issues)

---

## 📜 License

Proprietary software. The `.exe` releases are **free for personal use**. Redistribution or commercial use requires permission. Source code is not publicly available.

---

## 🙏 Credits

- [Ren'Py](https://www.renpy.org/) by Tom "PyTom" Rothamel — the visual novel engine
- [unrpyc](https://github.com/CensoredUsername/unrpyc) by CensoredUsername — `.rpyc` decompiler (MIT, vendored)
- [unrpa](https://github.com/Lattyware/unrpa) by Lattyware — `.rpa` extractor
- [deep-translator](https://github.com/nidhaloff/deep-translator) — Google Translate Python wrapper

---

<sub>**Keywords**: ren'py translator, visual novel translation, traduzir visual novel, tradutor renpy português, auto translate visual novel, free vn translator, vn pt-br, traducir visual novel, traductor renpy español, переводчик визуальных новелл, ren'py перевод, automatic localization, vn auto translate, free game translation, no API key translator.</sub>
