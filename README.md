# ToolPick

Небольшой SEO-сайт на английском: честные сравнения AI/SaaS-инструментов и платные цифровые материалы. Работает без хостинга и домена — только GitHub Pages.

## Быстрые ссылки

- **Живой сайт:** https://aleksei-ship-it.github.io/toolpick-site/
- **Короткий адрес** (сам перебрасывает на сайт): https://aleksei-ship-it.github.io/
- **Пример статьи:** https://aleksei-ship-it.github.io/toolpick-site/articles/best-ai-tools-for-bookkeepers/
- **Файлы сайта на GitHub:** https://github.com/Aleksei-ship-it/toolpick-site/tree/gh-pages
- **Репозиторий-редирект:** https://github.com/Aleksei-ship-it/Aleksei-ship-it.github.io

## Почему репозиторий кажется пустым

По умолчанию GitHub открывает ветку `main`, а в ней лежит только этот README. **Весь сайт находится в ветке `gh-pages`.**

Как посмотреть:
1. Откройте https://github.com/Aleksei-ship-it/toolpick-site
2. Над списком файлов нажмите выпадающий список `main branch`.
3. Выберите `gh-pages`.

Там будут папки `articles/`, `products/`, `go/`, `tools/ai-roi/`, `assets/`, `about/`, файлы `index.html`, `sitemap.xml`, `robots.txt`.

Исходный код генератора (`affiliate-engine/`) и платные ZIP-файлы **намеренно не публикуются** — они остаются на локальном компьютере. Иначе товары можно было бы скачать бесплатно.

## Как здесь зарабатывают

**1. Продажа цифровых товаров — уже работает.** Всего 10 товаров по `$9–$29`. Страница товара ведёт на платёжную ссылку Zypher; покупатель платит криптой (USDT/USDC/BTC и др.), деньги сразу приходят на внутренний баланс Zypher.

**2. Партнёрские комиссии — после одобрения заявок.** Сейчас ссылки `/go/<slug>/` ведут на официальные сайты и commission не приносят. Поданы заявки HubSpot (через Impact), Cloudways, Kit (PartnerStack), Trybit и Oxa Pay — как только их одобрят, заглушки заменяются на партнёрские ссылки.

## Что делать, когда придёт первая оплата

1. Проверка инвойсов запускается автоматически каждый день в **09:30 по Москве** (`Zypher Daily Sales Check`).
2. Откройте https://zypher.exchange/merchant → **Invoices**. В поле **Message** оплаченного инвойса будет email покупателя. Если email не указан, человек пишет в Telegram `@Alseamen`.
3. Возьмите ZIP из `products/<slug>/<slug>.zip` в локальной папке `affiliate-engine/` и отправьте файл со своей почты **в течение 24 часов**. На сайте честно обещано именно 24 часа.
4. Вывод денег на кошелёк делается только по вашей просьбе: нужен **только публичный адрес**. Seed-фразы, приватные ключи и данные карт никому не сообщаются.

## Реалистичные сроки

- Первые продажи товаров: от нескольких недель до 2–3 месяцев (сайт новый, трафик набирается).
- Стабильные продажи: ориентир 3–6 месяцев регулярных статей.
- Заметный доход: 6–12 месяцев.
- Партнёрские комиссии: после одобрения и первой покупки клиентом, обычно 30–60+ дней.

Сайт обновляется автоматически: статьи ежедневно, проверка оплат ежедневно, партнёрки еженедельно, отчёты ежемесячно.

## Как пересобрать и опубликовать

```bash
cd affiliate-engine
python build.py --check
python build.py
python deploy.py "описание изменений"
```

Публикация идёт в ветку `gh-pages`; GitHub Pages подтягивает изменения примерно за минуту. Секреты хранятся только локально в `config/secrets.local.json` и в репозиторий не попадают.


## Published write-ups and listings

- [DEV Community: The 5-Minute ROI Check I Run Before Paying for Another AI Tool](https://dev.to/toolpick/the-5-minute-roi-check-i-run-before-paying-for-another-ai-tool-5ak1)
- [Hashnode: same article on the ToolPick blog](https://toolpick.hashnode.dev/the-5-minute-roi-check-i-run-before-paying-for-another-ai-tool)
- [Indie Hackers: ToolPick product page](https://www.indiehackers.com/product/toolpick)
- [GitHub Discussion: ToolPick is live](https://github.com/Aleksei-ship-it/toolpick-site/discussions/1)
- [Substack: Why I started ToolPick](https://toolpick.substack.com/p/why-i-started-toolpick)
- [GitHub profile README](https://github.com/Aleksei-ship-it)

If these posts helped you, star the repo or share the [free ROI calculator](https://aleksei-ship-it.github.io/toolpick-site/tools/ai-roi/).
