# Открытки

Переходи ниже, выбирай любую понравившуюся открытку: на чёрном фоне распускается цветок, выстраивается созвездие, разворачивается письмо. Каждая принимает имя и текст в URL — то есть ссылку можно отправить персонально, без правки кода, самостоятельно, ниже инструкция.

**Демо (тут все открытки):** https://vincere-mori.github.io/love/

→ [English below](#cards)

## Что есть

| Открытка | Что происходит |
|---|---|
| [пион](https://vincere-mori.github.io/love/cards/pion/) | 3D-пион распускается и увядает. Мышь поворачивает в пространстве, колесо — раскручивает. |
| [созвездие](https://vincere-mori.github.io/love/cards/sozvezdie/) | Звёздное небо, из звёзд складывается сердце, под ним — имя. Падающие звёзды по клику. |
| [сердце](https://vincere-mori.github.io/love/cards/serdtse/) | ~2400 частиц в форме сердца, пульсирует, поворачивается. По клику рассыпается и собирается обратно. |
| [письмо](https://vincere-mori.github.io/love/cards/pismo/) | Бумажное письмо разворачивается, строки проявляются по очереди, в углу — сургучная печать. Пыль в луче света. |
| [светлячки](https://vincere-mori.github.io/love/cards/svetlyachki/) | Тёплый июльский вечер: светлячки летают по полю, тянутся к курсору, по клику собираются в сердце. |
| [часы](https://vincere-mori.github.io/love/cards/chasy/) | Циферблат из лент, в центре — имя и дата (для годовщины, например). |

## Как послать своей

Просто докинь параметры в URL:

```
https://vincere-mori.github.io/love/cards/sozvezdie/?name=Аня&text=моё небо
https://vincere-mori.github.io/love/cards/serdtse/?text=для тебя
https://vincere-mori.github.io/love/cards/pismo/?name=Милая&text=строка раз|строка два|строка три&sign=твой С.
https://vincere-mori.github.io/love/cards/svetlyachki/?name=Аня&text=наш июльский вечер
https://vincere-mori.github.io/love/cards/chasy/?name=Аня и Саша&date=14 февраля 2024&text=наша вечность
```

В письме строки разделяются `|`. Кириллица и пробелы — нормально (браузер сам закодирует), но если пересылаешь в мессенджере, лучше просто скопировать ссылку из адресной строки.

Всё статика, ничего никуда не уходит.

## Управление

- **мышь** — лёгкий доворот / параллакс
- **колесо мыши** — раскрутить пион
- **клик** — взрыв сердца / звёздный дождь / сборка светлячков (зависит от карточки)

## Сделать свою

Каждая открытка — один `index.html` + p5.js с CDN. Правишь файл в `cards/<имя>/index.html`, меняешь что хочешь. Цветовая схема пиона лежит массивом `blooms` в начале скрипта.

## Технически

- p5.js 1.9.3 с CDN
- HTML/CSS/JS, без сборки
- Работает на телефоне

## Поддержать

Если понравилось — поставь ⭐ и/или можешь отправить на чай:

- [Чаевые](https://pay.cloudtips.ru/p/6c077990)

## Лицензия

MIT. Если сделаешь свою открытку — кинь ссылку в issue, добавлю в галерею.

---

# Cards

Six animated cards in your browser, built with p5.js. A peony grows, fireflies drift, a letter opens. You pass the name and text in the URL and send the link — no code editing, no app, nothing to install.

**Live:** https://vincere-mori.github.io/love/

| Card | What it does |
|---|---|
| [peony](https://vincere-mori.github.io/love/cards/pion/) | 3D peony blooms and wilts. Move the mouse to rotate, scroll to spin. |
| [constellation](https://vincere-mori.github.io/love/cards/sozvezdie/) | Stars slowly form a heart with a name underneath. Click to trigger a shooting star shower. |
| [heart](https://vincere-mori.github.io/love/cards/serdtse/) | About 2400 particles in the shape of a beating heart. Click to shatter it and watch it pull back together. |
| [letter](https://vincere-mori.github.io/love/cards/pismo/) | A paper letter folds open, lines appear one by one, wax seal at the end. |
| [fireflies](https://vincere-mori.github.io/love/cards/svetlyachki/) | A warm night field. Fireflies follow the cursor, click to gather them into a heart. |
| [clock](https://vincere-mori.github.io/love/cards/chasy/) | A dial made of flowing ribbons, name and date in the center. Works well for anniversaries. |

## Personalize

Put params in the URL, open it, share it:

```
https://vincere-mori.github.io/love/cards/sozvezdie/?name=Anna&text=my sky
https://vincere-mori.github.io/love/cards/serdtse/?text=for you
https://vincere-mori.github.io/love/cards/pismo/?name=Dear&text=Line one|Line two|Line three&sign=yours
https://vincere-mori.github.io/love/cards/svetlyachki/?name=Anna&text=our July evening
https://vincere-mori.github.io/love/cards/chasy/?name=Anna+%26+Sasha&date=February+14+2024&text=our+eternity
```

Separate letter lines with `|`. Copy the URL from the address bar before sending — browser will encode it properly.

## Run it locally

```bash
git clone https://github.com/vincere-mori/love
cd love
python -m http.server 8000
```

## Tip

If you like it: [cloudtips](https://pay.cloudtips.ru/p/6c077990)

## License

MIT.
