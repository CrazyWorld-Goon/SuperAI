# Черновики постов (L1)

Публикация: агент пишет файл здесь → человек копирует на pikabu.ru → Publish. Автопубликации нет.

## Имена файлов

`YYYYMMDD-slug.md` (пример: `20260725-pervyy-post-pro-X.md`)

Шаблон: [`_TEMPLATE.md`](_TEMPLATE.md)

## Статусы в frontmatter

| status | Значение |
|--------|----------|
| `draft` | агент написал, человек ещё не смотрел |
| `approved` | человек ок, можно публиковать |
| `published` | выложено; заполнены `published_url`, `published_at` |
| `measured` | заполнены замер и `result` |
| `killed` | не публикуем / гипотеза отброшена |

## После Publish

1. Вписать `published_url`, `published_at`, `status: published`.
2. Через ~24ч — `pluses_24h`, `pluses_niche_median_24h`, `delta_subs`, `result` (`win` / `lose` / `unclear`), `status: measured`.
3. Файл не удалять: это лог обучения агента.
