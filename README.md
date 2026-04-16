[README.md](https://github.com/user-attachments/files/26800298/README.md)
# RESULTAT Family Office — Website

## Быстрый старт

### 1. GitHub — загрузить файлы

1. Зайди на **github.com** → New repository
2. Назови: `resultat-site`
3. Нажми "Add file" → "Upload files"
4. Загрузи оба файла: `index.html` и `vercel.json`
5. Нажми **Commit changes**

---

### 2. Vercel — запустить сайт

1. Зайди на **vercel.com** → Sign Up (через GitHub)
2. New Project → выбери репозиторий `resultat-site`
3. Нажми **Deploy**
4. Сайт готов по адресу: `resultat-site.vercel.app`

---

### 3. Привязать домен resultat.co.il (один раз навсегда)

#### В Vercel:
1. Зайди в свой проект → Settings → **Domains**
2. Введи: `resultat.co.il`
3. Нажми Add
4. Vercel покажет тебе DNS-записи (обычно два значения)

#### У регистратора домена (где купил .co.il):
Добавь две записи:

| Тип | Имя | Значение |
|-----|-----|---------|
| A   | @   | 76.76.21.21 |
| CNAME | www | cname.vercel-dns.com |

Через 1–24 часа сайт будет доступен по адресу `resultat.co.il`.

> **Важно:** Домен привязывается **один раз**. После этого любые изменения в коде (новый дизайн, тексты) — просто обновляешь файлы в GitHub, Vercel автоматически перезапускает сайт. Домен менять не нужно.

---

### 4. Подключить форму (Formspree)

1. Зайди на **formspree.io** → New Form
2. Получи свой Form ID (вида: `xabc1234`)
3. В файле `index.html` найди строку:
   ```
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
4. Замени `YOUR_FORM_ID` на свой ID
5. Сохрани и загрузи в GitHub

---

### 5. Обновить контактные данные

В файле `index.html` замени:
- `972000000000` → твой номер WhatsApp (без + и пробелов)
- `+972 00 000-0000` → твой номер для отображения
- `info@resultat.co.il` → твой email
- `@resultat_office` → твой Telegram

---

## Структура файлов

```
resultat-site/
├── index.html     # Весь сайт (один файл)
├── vercel.json    # Конфиг для Vercel
└── README.md      # Эта инструкция
```

---

## Функции

- ✅ Дизайн в стиле BlackRock (тёмный, премиальный)
- ✅ Glassmorphism карточки
- ✅ Шрифты: Cormorant Garamond + DM Sans
- ✅ Цвета: чёрный + золото (как BlackRock IL)
- ✅ Кнопка WhatsApp (навигация + форма)
- ✅ Кнопка телефона
- ✅ Форма обратной связи (Formspree)
- ✅ Кнопка доступности (требование израильского закона IS 5568)
- ✅ Skip-link для скринридеров
- ✅ Полная ARIA-разметка
- ✅ Мобильная версия
- ✅ Анимации при скролле
- ✅ Юридический дисклеймер (по закону Израиля)
