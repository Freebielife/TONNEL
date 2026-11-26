# Tonnel Network Token Observatory

## О проекте / токене

Самоописание TONNEL из метаданных контракта: “Tonnel Network is the first Zero-Knowledge powered project built on the TON blockchain that provides privacy features for TON, JETTONs and NFTs.” Это заявление проекта, оно не подтверждено независимо.

Проверка источника и контракта выполнена 2026-11-26.

- Метаданные контракта: https://tonapi.io/v2/jettons/EQDNDv54v_TEU5t26rFykylsdPQsv5nsSZaH_v7JSJPtMitv
- Официальный сайт: https://www.tonnel.network/
- Официальный Telegram: https://t.me/tonnel_en
- Контракт: `0:cd0efe78bff4c4539b76eab17293296c74f42cbf99ec499687fefec94893ed32`

## Обсерватория

Standalone страница `index.html` собирается командами `python3 -m scripts.refresh_observatory`, `python3 build.py` и `python3 verify.py`. HTML не загружает внешние шрифты, скрипты или изображения. Внешние API используются только при обновлении данных.

В конфигурации указаны три пула TON с подтверждёнными успешными обменами: DeDust и STON.fi. Основной пул выбирается по наибольшей индексируемой USD-ликвидности среди подтверждённых поддерживаемых пулов. В истории остаются пропуски, если источник не возвращает полное покрытие.

Обновление через workflow требует GitHub Actions и подключённого планировщика `workflow_dispatch`; запуск по расписанию проверяется отдельно. В последней локальной сборке не удалось обновить разделы доменов и номеров Fragment, остальные ключевые снимки собраны.

Версия основы: 1.3.0. Топ холдеров показывает 10 записей с раскрытием до 20.
