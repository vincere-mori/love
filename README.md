# love

Шесть генеративных открыток на p5.js. Растёт цветок, светятся светлячки, разворачивается письмо. Каждая принимает имя и текст прямо в URL — ссылку можно послать лично, без правки кода.

**Демо:** https://vincere-mori.github.io/love/

→ [English version below](#love-1)

---

## Что есть

| Открытка | Что происходит |
|---|---|
| [пион](cards/pion/) | 3D-пион из бутона в цветение, меняет режим отрисовки. Мышь крутит, колесо раскручивает. |
| [созвездие](cards/sozvezdie/) | Звёздное небо, из звёзд складывается сердце, под ним — имя. По клику — звёздный дождь. |
| [сердце](cards/serdtse/) | ~2400 частиц в форме сердца. Мышь вращает, клик — рассыпается и собирается обратно. |
| [письмо](cards/pismo/) | Бумажное письмо разворачивается, строки проявляются по одной, в углу — сургучная печать. |
| [светлячки](cards/svetlyachki/) | Светлячки дрейфуют по ночному полю. Мышь притягивает, клик — собирает в сердце. |
| [часы](cards/chasy/) | Циферблат из лент, в центре — имя и дата. Под годовщину или «просто так». |

## Как послать своей

Добавь параметры в URL:

```
cards/sozvezdie/?name=Аня&text=моё небо
cards/serdtse/?text=для тебя
cards/pismo/?name=Милая&text=строка раз|строка два|строка три&sign=твой А.
cards/svetlyachki/?name=Аня&text=ты светишься
cards/chasy/?name=Аня и Саша&date=14 февраля 2024&text=наша вечность
```

В письме строки разделяются `|`. Кириллица и пробелы — нормально (браузер сам закодирует). Все открытки — статика, ничего не отправляется на сервер.

## Управление

- **пион** — мышь крутит, колесо мыши раскручивает, `F` — полный экран
- **созвездие** — мышь: параллакс, клик — звёздный дождь
- **сердце** — мышь: поворот, клик — взрыв частиц
- **светлячки** — мышь: притягивает, клик — собрать в сердце

## Локально

```bash
git clone https://github.com/vincere-mori/love
cd love
python -m http.server 8000
# открой http://localhost:8000
```

## Сделать свою

Каждая открытка — один `index.html` в `cards/<имя>/`. Правишь файл — меняешь цвета, текст, геометрию. p5.js подключён с CDN, сборка не нужна.

## Поддержать

Если понравилось — поставь ⭐ и/или кинь немного:

- [Чаевые (cloudtips)](https://pay.cloudtips.ru/p/6c077990)
- [Boosty](https://boosty.to/jsu/donate)

## Лицензия

MIT. Бери, форкай, дари. Если сделаешь свою открытку — кинь ссылку в issue, добавлю в галерею.

---

# love

Six generative greeting cards built with p5.js. A peony blooms, fireflies drift, a letter unfolds. Each card reads a name and message from the URL — send a personalized link directly, no code needed.

**Demo:** https://vincere-mori.github.io/love/

## Cards

| Card | What it does |
|---|---|
| [peony](cards/pion/) | 3D peony that blooms and wilts, switches render modes. Mouse rotates, scroll wheel spins. |
| [constellation](cards/sozvezdie/) | Starry sky where stars form a heart with a name beneath. Click for a shooting star shower. |
| [heart](cards/serdtse/) | ~2400 particles shaped into a beating heart. Mouse rotates, click — it shatters and reforms. |
| [letter](cards/pismo/) | A paper letter unfolds, lines appear one by one, sealed with wax. |
| [fireflies](cards/svetlyachki/) | Fireflies drift across a night field. Mouse attracts them, click — they gather into a heart. |
| [clock](cards/chasy/) | A ribbon clock dial with a name and date in the center. Great for anniversaries. |

## Personalize via URL

```
cards/sozvezdie/?name=Anna&text=my sky
cards/serdtse/?text=for you
cards/pismo/?name=Dear&text=First line|Second line|Third line&sign=yours
cards/svetlyachki/?name=Anna&text=you glow
cards/chasy/?name=Anna %26 Sasha&date=February 14 2024&text=our eternity
```

Separate letter lines with `|`. Browser encodes special characters automatically. Everything is static — nothing is sent to a server.

## Controls

- **peony** — mouse rotates, scroll wheel spins, `F` — fullscreen
- **constellation** — mouse parallax, click — shooting stars
- **heart** — mouse rotates, click — particle burst
- **fireflies** — mouse attracts, click — form a heart

## Run locally

```bash
git clone https://github.com/vincere-mori/love
cd love
python -m http.server 8000
# open http://localhost:8000
```

## Support

If you like this project — star ⭐ it and/or tip:

- [Cloudtips](https://pay.cloudtips.ru/p/6c077990)
- [Boosty](https://boosty.to/jsu/donate)

## License

MIT. Fork it, use it, share it. If you build your own card — drop a link in the issues.
