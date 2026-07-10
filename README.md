# 💳 sbp-qr

Красивая статичная страница для получения переводов по СБП.

Полностью клиентская, без серверов. Работает на GitHub Pages.

**Workflow для деплоя настроен через GitHub Actions.**

## Как создать свою страницу

1. Перейдите: **https://6w2xjystnb-bot.github.io/sbp-qr/**
2. Заполните Фамилию, Имя, Отчество и телефон
3. Нажмите «Создать мою страницу»
4. Скопируйте ссылку или скачайте QR-код
5. Отправьте ссылку или QR кому угодно

Есть кнопка **«Посмотреть демо»** — сразу покажет, как выглядит готовая страница.

### Пример готовой страницы

https://6w2xjystnb-bot.github.io/sbp-qr/#d=JTdCJTIybmFtZSUyMiUzQSUyMCUyMiVEMCU5OCVEMCVCMiVEMCVCMCVEMCVCRCVEMCVCRSVEMCVCMiUyMCVEMCU5OCVEMCVCMiVEMCVCMCVEMCVCRCUyMCVEMCU5OCVEMCVCMiVEMCVCMCVEMCVCRCVEMCVCRSVEMCVCMiVEMCVCOCVEMSU4NyUyMiUyQyUyMCUyMnBob25lJTIyJTNBJTIwJTIyJTJCNzk5OTEyMzQ1NjclMjIlN0Q=

## На странице получателя

- В самом верху — большая кнопка копирования номера + инструкция «Зайдите в банк → Переводы → По номеру телефона (СБП)»
- Ниже — красивые карточки банков. Клик → диплинк + копирование номера

## Если сайт ещё не работает (404)

Зайди один раз в репозиторий:

**Settings → Pages**

Выбери Source: **GitHub Actions**

Затем зайди в **Actions** tab и запусти или подожди первый запуск workflow.

После этого сайт появится.

## Технические детали

- Однофайловое приложение (`index.html`)
- Tailwind + QRCode.js через CDN
- Данные кодируются в hash URL (`#d=...`)
- Никаких запросов на сервер

Можно использовать как есть или форкнуть и кастомизировать.
