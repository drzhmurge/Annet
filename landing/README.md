# Annet Cloud — Landing Page

Лендинг-прокладка для рекламных баннеров. Чистый HTML + CSS, деплой на GitHub Pages.

## Структура

```
landing/
  index.html        — разметка страницы
  style.css         — стили
  assets/
    logo.png        — логотип
    fox.png         — персонаж Annet Fox
    bg.jpg          — фон hero-секции
    qr-proxy-1.png  — QR-код прокси #1
    qr-proxy-2.png  — QR-код прокси #2
```

## Секции

1. **Hero** — заголовок + CTA → Telegram-бот
2. **Features** — преимущества сервиса + тарифы
3. **Как подключиться** — 3 шага
4. **MTProto прокси** — для пользователей с заблокированным Telegram
5. **Footer**

## MTProto прокси

| # | Сервер | Порт | Ссылка |
|---|--------|------|--------|
| 1 | 158.160.62.185 | 9443 | `tg://proxy?server=158.160.62.185&port=9443&secret=156c55e42c5e8cfccc443581554e3a96` |
| 2 | 158.160.59.192 | 9443 | `tg://proxy?server=158.160.59.192&port=9443&secret=156c55e42c5e8cfccc443581554e3a96` |

## Деплой

Автодеплой через GitHub Actions при `push` в `main` (изменения в `landing/**`).

Для ручного деплоя: вкладка **Actions → Deploy Landing to GitHub Pages → Run workflow**.

### Настройка GitHub Pages (один раз)

1. Settings → Pages → Source: **GitHub Actions**
2. Запушить изменения в `main`
3. Страница будет доступна по адресу `https://<org>.github.io/<repo>/`
