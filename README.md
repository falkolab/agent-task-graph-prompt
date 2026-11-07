# AI Agent Task Graph — Parallel Execution, Validation & Recovery (EN/RU)

A graph-oriented prompt for autonomous AI agents. The same structure is presented in English and Russian, with English XML tags and variables in both versions.

## Versions

- [English — prompt.en.md](prompt.en.md): English **reconstruction** from a Spanish-language graphic, *not independently verified against the author's full original English prompt*.
- [Русский — prompt.ru.md](prompt.ru.md): перевод текста с испаноязычного изображения с сохранением смысла, структуры и файловых артефактов.

### Fidelity / Точность

Checked against the supplied Spanish-language image (15 XML blocks: outer prompt + 14 sections). The `checks.md` ledger requirement is retained. XML tag names and placeholders are normalized into English, and the inconsistent spelling of `{{LIMITE}}` / `{{LÍMITE}}` is unified as `{{LIMIT}}`. This is an editorial translation/reconstruction, **not a verbatim reproduction of the original English author comment**.

Содержимое сверено с изображением. Исправлен пропуск требования записывать результаты проверок в `checks.md`, по одной строке на требование. Названия XML-тегов и переменных нормализованы; `{{LIMITE}}` / `{{LÍMITE}}` заменены единым `{{LIMIT}}`. Дословное совпадение с исходным англоязычным комментарием автора **не подтверждено**.

## How to use / Применение

Fill in / заполните: `{{TASK}}`, `{{OUTPUT}}`, `{{CHECKS}}`, `{{SOURCES}}`, `{{SCOPE}}`, `{{LIMIT}}`. Agent runtime must support delegation, file persistence, deterministic checks, and explicit approval for risky actions. **A prompt alone does not guarantee reliable execution.**

## Attribution / Источники

- Idea / original social post: [Hoodie (@HoodieFade_), 4 November 2026](https://x.com/HoodieFade_/status/2118010863038746652).
- Methodological inspiration: [Andrej Karpathy — autoresearch](https://github.com/karpathy/autoresearch).
- RU translation, EN reconstruction, editorial normalization: Андрей Ткаченко, «Автоматизируй это» · [@aitomateit](https://t.me/aitomateit).

This prompt is not authored by Andrej Karpathy. / Этот промпт написан не Андреем Карпати.