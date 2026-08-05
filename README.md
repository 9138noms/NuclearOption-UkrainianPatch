# Nuclear Option — Український патч (Localization Patch)

Мод української локалізації для Nuclear Option. Працює як плагін BepInEx і перекладає інтерфейс, енциклопедію, підказки й випливаючі описи — загалом **2 084 записи**.

## Вимоги

- [Nuclear Option](https://store.steampowered.com/app/2230590/Nuclear_Option/) (Steam, Ранній доступ 0.34)
- [BepInEx 5.x](https://github.com/BepInEx/BepInEx/releases)

## Встановлення

1. Установіть **BepInEx 5.x** у папку гри.
   ```
   Приклад: C:\Program Files (x86)\Steam\steamapps\common\Nuclear Option\
   ```

2. Запустіть гру **один раз** і закрийте її. (Це створить структуру папок BepInEx.)

3. Скопіюйте всі файли з цього репозиторію до:
   ```
   [Папка гри]\BepInEx\plugins\LocalizationPatch\
   ```
   > Якщо папки «LocalizationPatch» немає, створіть її вручну.

4. Запустіть гру — **український переклад застосується автоматично**.

### Автоматичний інсталятор (альтернатива)

https://github.com/9138noms/NuclearOption-LocalizationInstaller/releases/latest

## Включені файли

| Файл | Опис |
|------|------|
| `LocalizationPatch.dll` | Плагін перекладу |
| `ua.json` | Дані українського перекладу (2 084 записи) |
| `Exo2-Regular.ttf` | Шрифт для відображення кирилиці (використовується) |
| `Tektur-Reg.ttf` | Попередній шрифт, залишено для сумісності |

## Гарячі клавіші у грі

| Клавіша | Функція |
|---------|---------|
| `F10` | Показати/приховати оверлей налагодження |
| `Ctrl+F10` | Перезавантажити дані перекладу (гаряче перезавантаження) |

## Примітки

- Назви фракцій (PALA, BDF, BOSCALI, PRIMEVA, FFL, LMA) і кодові імена техніки / зброї (Compass, Alkyon AB-4, FGA-57 Anvil, IRM-S2 тощо) залишаються англійською.
- У разі проблем мову можна вказати вручну у файлі `BepInEx\config\com.noms.localizationpatch.cfg`, установивши `Language = ua`.

## Переклад

- Початковий машинний переклад — виправлення від спільноти вітаються через PR або Issue.
- Плагін / основа: https://github.com/9138noms/NuclearOption-TranslationToolkit

## Ліцензія шрифту

Tektur — [SIL Open Font License 1.1](https://fonts.google.com/specimen/Tektur)

## Source code

This mod ships `LocalizationPatch.dll`, a BepInEx plugin. Its full source is published
at **https://github.com/9138noms/NuclearOption-LocalizationPatch** — no obfuscation, no network access, no code outside the game folder.

The same plugin binary is shared by every language patch; only the `.json` and the font
differ between them.
