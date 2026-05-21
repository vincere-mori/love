# Открытки

Переходи ниже, выбирай любую понравившуюся открытку: на чёрном фоне распускается цветок, выстраивается созвездие, разворачивается письмо. Каждая принимает имя и текст в URL — то есть ссылку можно отправить персонально, без правки кода, самостоятельно, ниже инструкция.

**Демо (тут все открытки):** https://vincere-mori.github.io/love/

→ [English version below](#cards)

## Что есть

| Открытка | Что происходит |
|---|---|
| [пион](cards/pion/) | 3D-пион распускается и увядает. Мышь поворачивает в пространстве, колесо — раскручивает. |
| [созвездие](cards/sozvezdie/) | Звёздное небо, из звёзд складывается сердце, под ним — имя. Падающие звёзды по клику. |
| [сердце](cards/serdtse/) | ~2400 частиц в форме сердца, пульсирует, поворачивается. По клику рассыпается и собирается обратно. |
| [письмо](cards/pismo/) | Бумажное письмо разворачивается, строки проявляются по очереди, в углу — сургучная печать. Пыль в луче света. |
| [светлячки](cards/svetlyachki/) | Тёплый июльский вечер: светлячки летают по полю, тянутся к курсору, по клику собираются в сердце. |
| [часы](cards/chasy/) | Циферблат из лент, в центре — имя и дата (для годовщины, например). |

## Как послать своей

Просто докинь параметры в URL:

```
.../cards/sozvezdie/?name=Аня&text=моё небо
.../cards/serdtse/?text=для тебя
.../cards/pismo/?name=Милая&text=строка раз|строка два|строка три&sign=твой С.
.../cards/svetlyachki/?name=Аня&text=наш июльский вечер
.../cards/chasy/?name=Аня и Саша&date=14 февраля 2024&text=наша вечность
```

В письме строки разделяются `|`. Кириллица и пробелы — нормально (браузер сам закодирует), но если пересылаешь в мессенджере, лучше просто скопировать готовую ссылку из адресной строки.

Все ссылки — статика, ничего не отправляется на сервер, ничего не сохраняется. Открытка живёт только в URL.

## Управление

- **мышь** — лёгкий доворот / параллакс
- **колесо мыши** — раскрутить пион
- **клик** — взрыв сердца / звёздный дождь / сборка светлячков (зависит от карточки)
- **F** в пионе — полный экран

## Сделать свою

Каждая открытка — один `index.html` + p5.js с CDN. Если хочешь переписать текст, поменять палитру или геометрию — правишь файл в `cards/<имя>/index.html`. Цветовая схема пиона лежит массивом `blooms` в начале, для остальных — параметры рядом с инициализацией. Палитры превью на витрине — в `index.html` корня в CSS-классах `.pion .art` и т.д.

## Технически

- p5.js 1.9.3 с CDN
- Чистый HTML/CSS/JS, ноль зависимостей кроме p5
- Работает на телефоне, респонсив через `vw`-юниты

## Поддержать

Если понравилось — поставь ⭐ и/или можешь отправить на чай:

- [Чаевые (cloudtips)](https://pay.cloudtips.ru/p/6c077990)
- [Boosty](https://boosty.to/jsu/donate)

## Лицензия

MIT. Если сделаешь свою открытку — кинь ссылку в issue, добавлю в галерею.

---

# Cards

Six generative cards built with p5.js. A peony blooms, fireflies drift, a letter unfolds. Each card reads a name and message straight from the URL — send a personalized link, no code needed.

**Demo (all cards here):** https://vincere-mori.github.io/love/

## What's inside

| Card | What it does |
|---|---|
| [peony](cards/pion/) | 3D peony blooms and wilts. Mouse rotates it, scroll wheel spins it. |
| [constellation](cards/sozvezdie/) | Stars form a heart with a name beneath. Click for a shooting star shower. |
| [heart](cards/serdtse/) | ~2400 particles pulsing in a heart shape. Mouse rotates, click — it shatters and reforms. |
| [letter](cards/pismo/) | A paper letter unfolds, lines appear one by one, sealed with wax. Dust in a beam of light. |
| [fireflies](cards/svetlyachki/) | Warm July evening: fireflies drift, follow the cursor, click — they form a heart. |
| [clock](cards/chasy/) | A ribbon clock dial with a name and date in the center. Great for anniversaries. |

## Send it to her

Add parameters to the URL:

```
.../cards/sozvezdie/?name=Anna&text=my sky
.../cards/serdtse/?text=for you
.../cards/pismo/?name=Dear&text=Line one|Line two|Line three&sign=yours
.../cards/svetlyachki/?name=Anna&text=our July evening
.../cards/chasy/?name=Anna %26 Sasha&date=February 14 2024&text=our eternity
```

Separate letter lines with `|`. Just copy the URL from the address bar — browser handles encoding. Everything is static, nothing is sent to a server.

## Controls

- **mouse** — gentle rotation / parallax
- **scroll wheel** — spin the peony
- **click** — heart burst / shooting stars / firefly heart (depends on the card)
- **F** on the peony — fullscreen

## Run locally

```bash
git clone https://github.com/vincere-mori/love
cd love
python -m http.server 8000
# open http://localhost:8000
```

## Make your own

Each card is a single `index.html` + p5.js from CDN. Edit `cards/<name>/index.html` to change colors, text, geometry. No build step.

## Support

If you like this — star ⭐ the repo and/or tip:

- [Cloudtips](https://pay.cloudtips.ru/p/6c077990)
- [Boosty](https://boosty.to/jsu/donate)

## License

MIT. Fork it, use it, share it. If you make your own card — drop a link in the issues.
