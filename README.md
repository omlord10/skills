# Портфолио навыков

Статическая страница без JavaScript и внешних запросов. Все картинки в `site/img/`
нарисованы вручную в SVG на тестовых данных (домены `example.com`,
адреса `203.0.113.0/24` из RFC 5737).

## Посмотреть локально

    python3 -m http.server -d site 8000
    # открыть http://localhost:8000

## Публикация

1. Создать репозиторий на GitHub и запушить ветку `main`.
2. Settings → Pages → Source: **GitHub Actions**.
3. Workflow `.github/workflows/pages.yml` соберёт и опубликует только папку `site/`.
   Если в `site/` окажется что-то кроме html/css/svg, деплой остановится.
