# 🚀 Команды для загрузки на GitHub

## Шаг 1: Проверьте текущий remote

```bash
cd /home/ubuntu/aurora
git remote -v
```

Если remote уже есть (origin), переходите к шагу 3.

## Шаг 2: Создайте репозиторий на GitHub

1. Перейдите на https://github.com/new
2. Название: `ThunderBolt-Launcher` (или любое другое)
3. Выберите **Public** или **Private**
4. **НЕ** добавляйте README, .gitignore или license (они уже есть)
5. Нажмите "Create repository"

## Шаг 3: Добавьте remote (если нужно)

```bash
# Замените USERNAME на ваш GitHub username
git remote add origin https://github.com/USERNAME/ThunderBolt-Launcher.git

# Или если remote уже есть, обновите его:
git remote set-url origin https://github.com/USERNAME/ThunderBolt-Launcher.git
```

## Шаг 4: Подготовьте файлы

```bash
cd /home/ubuntu/aurora

# Добавьте все изменения
git add .

# Создайте коммит
git commit -m "ThunderBolt Launcher - настроен сервер и клиент"
```

## Шаг 5: Загрузите на GitHub

```bash
# Если это первый push
git push -u origin master

# Или если ветка называется main
git push -u origin main

# Если возникают конфликты, используйте:
git push -u origin master --force
```

## Шаг 6: Запустите GitHub Actions

1. Перейдите на https://github.com/USERNAME/ThunderBolt-Launcher
2. Откройте вкладку **Actions**
3. Нажмите **"Build Windows Launcher"** в левом меню
4. Нажмите **"Run workflow"** справа
5. Выберите ветку `master` (или `main`)
6. Нажмите зеленую кнопку **"Run workflow"**

## Шаг 7: Скачайте готовый .exe

1. Дождитесь завершения сборки (~10-15 минут)
2. Когда увидите зеленую галочку ✅ - сборка завершена
3. Нажмите на completed workflow
4. Прокрутите вниз до **Artifacts**
5. Скачайте **ThunderBolt-Launcher-Windows**
6. Распакуйте архив - внутри будет `ThunderBolt-Launcher-0.0.4.exe`

## 🔐 Важно!

**Конфигурация с паролями MySQL НЕ попадет в репозиторий** - она в `.gitignore`.

Если нужно добавить пример конфига (без паролей), создайте:
- `packages/server/dist/LauncherServerConfig.hjson.example`

---

## 📝 Быстрые команды (скопируйте и выполните):

```bash
cd /home/ubuntu/aurora
git add .
git commit -m "ThunderBolt Launcher готов к сборке"
git push -u origin master
```

Затем на GitHub: Actions → Run workflow → Скачать Artifacts
