# Трекер звичок

Сторінка на GitHub Pages, дані у Firebase (Firestore). Вхід через Google,
галочки однакові на ПК і телефоні.

## Підключення Firebase (один раз, ~10 хв)

1. Відкрий https://console.firebase.google.com → **Create a project** (Додати проєкт).
   Назва, наприклад, `habit-tracker`. Google Analytics можна вимкнути.
2. **Build → Authentication → Get started → Sign-in method → Google → Enable**,
   вибери свою пошту як support email → Save.
3. Там же: **Authentication → Settings → Authorized domains → Add domain**:
   `vasyld-automation.github.io`.
4. **Project settings** (шестерня) → **Your apps** → іконка `</>` (Web) →
   назва будь-яка, Hosting НЕ вмикати → **Register app**. Скопіюй об'єкт
   `firebaseConfig` і встав його значення у файл `firebase-config.js`.
5. **Build → Firestore Database → Create database** → регіон `eur3 (europe-west)`
   → **Start in production mode** → Create.
6. Firestore → вкладка **Rules** → встав вміст файлу `firestore.rules` → **Publish**.

## GitHub Pages

Repo → **Settings → Pages** → Source: *Deploy from a branch*, гілка `main`, папка `/ (root)`.
Адреса: https://vasyld-automation.github.io/habit-tracker/

## На телефон

Відкрий адресу → увійди через Google → меню браузера → **Додати на головний екран**.
