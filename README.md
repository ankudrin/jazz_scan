# jazz_scan





```
jazz_scan/
├── cmd/                          # Исполняемые файлы
│   ├── webrecon/                 # CLI утилита
│   └── webrecon-server/          # API сервер
├── internal/                     # Внутренние пакеты
│   ├── core/                     # Ядро системы
│   │   ├── config/               # Конфигурация
│   │   ├── pipeline/             # Процессор пайплайна
│   │   ├── project/              # Управление проектами
│   │   ├── scope/                # Управление scope
│   │   └── run/                  # Управление запусками
│   ├── stages/                   # Реализация этапов
│   │   ├── w1_ingest/            # W1: IngestNormalizeScope
│   │   ├── w2_passive/           # W2: PassiveDiscovery
│   │   ├── ...                   # W3-W10
│   │   └── w11_reporting/        # W11: ReportingAndExport
│   ├── model/                    # Модели данных (ontology)
│   │   ├── asset/                # Модели активов
│   │   ├── dns/                  # DNS модели
│   │   ├── net/                  # Сетевые модели
│   │   ├── web/                  # Веб-модели
│   │   └── sec/                  # Модели безопасности
│   ├── rules/                    # Движок правил
│   │   ├── engine/               # Ядро правил
│   │   └── packs/                # Наборы правил по категориям
│   ├── storage/                  # Хранилище
│   │   ├── postgres/             # Postgres адаптер
│   │   ├── s3/                   # S3 адаптер
│   │   └── search/               # Search адаптер (опционально)
│   └── exporters/                # Экспортеры
│       ├── sarif/                # SARIF экспортер
│       ├── stix/                 # STIX экспортер
│       └── html/                 # HTML отчеты
├── pkg/                          # Публичные пакеты
│   ├── api/                      # API клиент
│   ├── utils/                    # Утилиты
│   ├── validators/               # Валидаторы
│   └── scanners/                 # Сканеры и адаптеры
├── api/                          # API спецификация
│   └── openapi.yaml              # OpenAPI спецификация
├── schemas/                      # JSON Schema для артефактов
│   ├── targets.normalized.v1.json
│   ├── ...
│   └── findings.enriched.v1.json
├── config/                       # Примеры конфигураций
├── deploy/                       # Deployment конфигурации
│   ├── docker/                   # Docker файлы
│   └── compose/                  # Docker-compose файлы
├── scripts/                      # Вспомогательные скрипты
├── docs/                         # Документация
└── tests/                        # Тесты
    ├── unit/                     # Модульные тесты
    ├── integration/              # Интеграционные тесты
    └── acceptance/               # Приемочные тесты
```
