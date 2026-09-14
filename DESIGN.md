# DESIGN.md — University Website: Education Design Case

Документация дизайн-проекта сайта университета, выполненного в образовательной (education) тематике. Материал подготовлен на основе презентации проекта (Dribbble shot) и включает описание концепции, принципов дизайна и все опубликованные медиа-материалы.

## 1. Концепция

> «Корни образования горьки, но плоды его сладки» — Аристотель

Проект вдохновлён темой образования: сайт университета, который должен быть **аккуратным и функциональным**, **дружелюбным и информативным**, с положительным пользовательским опытом (UX), который строится на:

- прочной композиции и визуальной иерархии;
- продуманной компоновке контента;
- плавной анимации переходов и элементов.

## 2. Принципы дизайна

| Принцип | Реализация |
|---|---|
| Визуальная иерархия | Чёткое разделение блоков контента, крупные акцентные медиа-блоки |
| Дружелюбность | Мягкая цветовая гамма, скруглённые углы (`border-radius: 8px`) |
| Информативность | Комбинация коротких текстовых блоков и наглядных превью экранов |
| Живость интерфейса | Анимированные видео-превью (autoplay/loop) вместо статичных скриншотов |
| Отзывчивость (responsive) | Раздельные стили для десктопа (`large`) и мобильных (`small`) с адаптацией отступов, радиусов и ширины |

## 3. Стилевые константы

Извлечено из вёрстки презентации проекта:

- **Шрифт:** `"Mona Sans", "Helvetica Neue", Helvetica, Arial, sans-serif`
- **Базовый размер текста:** `16px`, заголовочные параграфы — `20px / 32px` (desktop), `16px / 28px` (mobile)
- **Начертание:** `font-weight: 400`, `font-style: normal`
- **Фон страницы:** `#FFFFFF`
- **Радиус скругления медиа-блоков:** `8px` (desktop), `0px` — full-bleed на мобильных
- **Максимальная ширина медиа-блока:** `1024px`, текстового блока — `752px`
- **Соотношение сторон медиа:** видео — `4:3`, изображения — `4:3` (3200×2400)
- **Брейкпоинты:** `large` (десктоп) и `small` (мобильный, full-width с отрицательными полями `calc(100% + 32px)`)

## 4. Медиа-материалы проекта

Ниже — все экраны/анимации, представленные в кейсе, в порядке появления.

### 4.1 Видео-превью (анимированные демонстрации интерфейса)

| # | Превью (poster) | Видео |
|---|---|---|
| 1 | [poster](https://cdn.dribbble.com/userupload/3006585/file/still-3a61a582310ff5f4b715b56b1d7a35a4.png) | [mp4](https://cdn.dribbble.com/userupload/3006585/file/original-47c62b9c0b48b05fc1e39d15a889bc8a.mp4) |
| 2 | [poster](https://cdn.dribbble.com/userupload/3006586/file/still-d06184d7ddbc98b80c65b1c268a86cba.png) | [mp4](https://cdn.dribbble.com/userupload/3006586/file/original-07b89d36d05f95eb7b1de8b2a3b66c62.mp4) |
| 3 | [poster](https://cdn.dribbble.com/userupload/3006592/file/still-7ff13706b97ef00870eb6da3091c4966.png) | [mp4](https://cdn.dribbble.com/userupload/3006592/file/original-b49b63180694b423b931cf2eefb988a5.mp4) |
| 4 | [poster](https://cdn.dribbble.com/userupload/3006589/file/still-35d83c9936abde720c8cadcd00d2e1d1.png) | [mp4](https://cdn.dribbble.com/userupload/3006589/file/original-ab6e6388532f8fef8d9d92854f702ad5.mp4) |
| 5 | [poster](https://cdn.dribbble.com/userupload/3006595/file/still-460ce1dcc0017125155b3e19acbe55c6.png) | [mp4](https://cdn.dribbble.com/userupload/3006595/file/original-392126c2dbd3294ab08d375824558b09.mp4) |
| 6 | [poster](https://cdn.dribbble.com/userupload/3006593/file/still-caa589bd6b46b7f8f235a3232ab890bd.png) | [mp4](https://cdn.dribbble.com/userupload/3006593/file/original-9100dc6fe3480e694767ad0e7ae3e8f7.mp4) |

Все видео воспроизводятся автоматически, зациклены (`loop`), без звука (`muted`), с возможностью паузы по клику (`toggle-play-on-click`).

### 4.2 Статичные экраны (изображения интерфейса)

| # | Alt-текст | Изображение |
|---|---|---|
| 1 | — | [PNG](https://cdn.dribbble.com/userupload/3006590/file/original-751bcba1e459d9fb6d53be92f6c1e98c.png) |
| 2 | education university website design | [PNG](https://cdn.dribbble.com/userupload/3006591/file/original-2a5a1f741be00442c2550b26e966b11e.png) |
| 3 | — | [PNG](https://cdn.dribbble.com/userupload/3006594/file/original-9c0b38fd5df0fb7444063b7d500600ee.png) |
| 4 | — | [PNG](https://cdn.dribbble.com/userupload/3006587/file/original-eb0b59d0d774cb016dd3585a4da9a781.png) |
| 5 | — | [PNG](https://cdn.dribbble.com/userupload/3006596/file/original-397235558dc947675276262db65039cd.png) |
| 6 | university website design | [PNG](https://cdn.dribbble.com/userupload/3006588/file/original-d3d3cbb35c8eb78cd143e29cb8d12b80.png) |

Исходное разрешение изображений — 3200×2400 (соотношение 4:3), отображаются с `object-fit: contain`.

## 5. Структура блока презентации

Каждый медиа-блок (видео или изображение) обёрнут в единообразный контейнер:

```
div (max-width 1024px, border-radius 8px, overflow hidden)
 └─ div (aspect-ratio 4:3)
     └─ div (по центру, height 100%)
         └─ video / image (border-radius 8px, object-fit: contain)
```

Текстовые блоки (цитата, описание, закрывающий призыв) используют более узкий контейнер (`max-width: 752px`) для комфортной ширины строки при чтении.

## 6. Примечание об источнике

Итоговый список кейса в оригинале обрывается на пункте «Also, welcome to check:» — ссылки на смежные работы отсутствуют в исходных данных и не были восстановлены в этом документе.
