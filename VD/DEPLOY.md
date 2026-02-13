# Безкоштовний деплой валентинки

Обери один із варіантів. Усі безкоштовні.

---

## 1. Netlify Drop (найпростіше, без реєстрації)

1. Відкрий у браузері: **https://app.netlify.com/drop**
2. Якщо попросить — зареєструйся (email або GitHub, безкоштовно).
3. Перетягни **папку** `VD` (та, де лежить `index.html`; якщо є `preview-gifs.html` і `assets` — теж перетягни всю папку) у вікно браузера.
4. Netlify дасть посилання типу `https://random-name-123.netlify.app` — ним можна ділитися.

**Плюси:** без терміналу, без git, за хвилину.

---

## 2. GitHub Pages (через репозиторій)

1. Зареєструйся на **https://github.com** (якщо ще немає).
2. Створи новий репозиторій (New repository), назва будь-яка, наприклад `valentine`.
3. У папці `VD` відкрий термінал і виконай:

```powershell
cd "c:\Users\Your Majesty\Downloads\VD\VD"
git init
git add index.html
git commit -m "Valentine page"
git branch -M main
git remote add origin https://github.com/ТВІЙ_ЛОГІН/valentine.git
git push -u origin main
```

(замість `ТВІЙ_ЛОГІН/valentine` — твоє ім’я на GitHub і назва репо).

4. На GitHub: **Settings** → **Pages** → Source: **Deploy from a branch** → Branch: **main** → **Save**.
5. Через хвилину сайт буде тут: `https://ТВІЙ_ЛОГІН.github.io/valentine/`

**Плюси:** своє посилання, можна оновлювати через `git push`.

---

## 3. Surge (одна команда в терміналі)

1. Встанови Node.js з **https://nodejs.org** (LTS), якщо ще немає.
2. У терміналі:

```powershell
cd "c:\Users\Your Majesty\Downloads\VD\VD"
npx surge . --domain valentine-кирил.surge.sh
```

3. Введи email і придумай пароль (створиться акаунт Surge).
4. Сайт з’явиться за посиланням типу `https://valentine-кирил.surge.sh`

**Плюси:** дуже швидко, з консолі.

---

## Рекомендація

Якщо не хочеш нічого встановлювати — використовуй **Netlify Drop** (варіант 1).  
Якщо є акаунт GitHub і хочеш мати репо — **GitHub Pages** (варіант 2).
