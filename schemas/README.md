# Схемы данных

Все схемы используют JSON Schema Draft 2020-12. Они применимы к JSON и к эквивалентным YAML-записям после разбора YAML.

| Схема | Объект |
|---|---|
| [`construct.schema.json`](construct.schema.json) | онтология PENTABASIS-LLM |
| [`source-registry.schema.json`](source-registry.schema.json) | библиографический и нормативный реестр |
| [`crosswalk.schema.json`](crosswalk.schema.json) | карта нормативного источника к PENTABASIS-LLM |
| [`item.schema.json`](item.schema.json) | каноническая ситуация и две формы протокола |
| [`response.schema.json`](response.schema.json) | неизменяемый первичный ответ модели |
| [`annotation.schema.json`](annotation.schema.json) | атомарная экспертная или автоматическая метка |
| [`run-manifest.schema.json`](run-manifest.schema.json) | воспроизводимый манифест прогона |

Схемы версионируются независимо от данных. Несовместимое изменение повышает основную версию `schema_version`.
