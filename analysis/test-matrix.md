# Матрица проверки

Desktop использует ширинный Auto Scale: scale = viewportWidth / 1200, как в Tilda. Высота рабочей области растёт пропорционально, поэтому элементы не остаются маленькими на широких экранах. До 900 px включается flow-компоновка.

| Разрешение | Режим | Масштаб рабочей области | Масштаб Canvas 1280×720 | Горизонтальный spill |
|---|---|---:|---:|---|
| 1280×720 | небольшой монитор / desktop width autoscale | 1.067 | 1.000 | нет |
| 1366×768 | ноутбук / desktop width autoscale | 1.138 | 1.067 | нет |
| 1440×900 | 16:10 / desktop width autoscale | 1.200 | 1.250 | нет |
| 1920×1080 | Full HD / desktop width autoscale | 1.600 | 1.500 | нет |
| 2560×1440 | QHD / desktop width autoscale | 2.133 | 2.000 | нет |
| 3840×2160 | 4K / desktop width autoscale | 3.200 | 3.000 | нет |
| 3440×1440 | UltraWide / desktop width autoscale | 2.867 | 2.688 | нет |
| 768×1024 | планшет / mobile/tablet flow | 1.000 | 1.422 | нет |
| 390×844 | смартфон / mobile/tablet flow | 1.000 | 1.172 | нет |

## Браузерные проверки

- JavaScript синтаксис: node --check — OK.
- HTML-парсинг: html.parser — OK.
- Кэш кадров: максимум 12 декодированных изображений; загружаются якоря и соседние кадры по мере движения.
- Встроенный browser preview в текущем окружении не смог открыть loopback-сервер (ERR_CONNECTION_TIMED_OUT), поэтому автоматические screenshots и замеры консоли здесь не получены.

Контактный лист всех кадров: analysis/contact/contact-sheet.jpg.