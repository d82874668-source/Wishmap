# Наша карта желаний

Сайт для двоих: желания с прогрессом, воспоминания, места, задания, магазин с монетами, реферальная программа, темы оформления.

## 1. База данных (Firebase)
1. console.firebase.google.com → Create a project (аналитику можно отключить).
2. Build → Firestore Database → Create database → Production.
3. Вкладка Rules: вставьте содержимое файла `firestore.rules` и нажмите Publish.
4. Build → Authentication → Get started → Sign-in method → включите Email/Password.
5. Authentication → Users → Add user: email администратора (`zubaka2802@mail.ru`) и ваш пароль.
6. Project settings (шестерёнка) → Your apps → значок `</>` → Register app → скопируйте `firebaseConfig`.

## 2. Настройки в сайте
Откройте `index.html` и в самом начале скрипта найдите блок `const FB={...}`. Подставьте значения:
apiKey, authDomain, projectId, storageBucket, messagingSenderId, appId.
Пока `projectId` пустой, сайт работает без общей базы (данные только в вашем браузере).

## 3. Публикация на GitHub Pages
1. Распакуйте архив. Загрузите файлы `index.html`, `README.md`, `firestore.rules` и `.nojekyll` в репозиторий (Add file → Upload files → Commit changes).
2. Settings → Pages → Branch: `main`, папка `/ (root)` → Save.
3. Через 1–2 минуты появится ссылка вида `https://ваш-ник.github.io/имя-репозитория/`.

## 4. Как пользоваться
- Первый вход: «Создать нашу карту». Кнопка «Позвать партнёра» в «Заданиях» даёт ссылку на общую карту.
- «Отправить приглашение»: друг получает 150 монет, вы 50.
- Админ (вход под email администратора) видит «∞» монет.
