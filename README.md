<p align="center"><img src="./logo.png" width="200px" height="200px"></p>
<h1 align="center">Aurora Launcher</h1>

## Модули

|           Название модуля           |             Описание              | Расположение                                                |
| :---------------------------------: | :-------------------------------: | ----------------------------------------------------------- |
|        @aurora-launcher/api         |    Библиотека для работы с API    | [packages/api](packages/api)                                |
|        @aurora-launcher/core        |     Библиотека с общим кодом      | [packages/core](packages/core)                              |
| @aurora-launcher/esbuild-decorators | Поддержка декораторов для esbuild | [packages/esbuild-decorators](packages/esbuild-decorators)  |
|      @aurora-launcher/launcher      |           Код лаунчера            | [packages/launcher](https://github.com/AuroraTeam/Launcher) |
|       @aurora-launcher/server       |         Код лаунчсервера          | [packages/server](packages/server)                          |

---

На данный момент лаунчер находится в разработке, но вы можете помочь мне с кодом или ведением задач. Или например предлагать свои идеи в раздел [Issues](https://github.com/AuroraTeam/LauncherServer/issues).
А также вы можете поддержать меня материально:

-   Перевод на карту: `4276 3000 2167 4414`

## Мы в Discord

[![](https://discord.com/api/guilds/730131402636525688/embed.png?style=banner2)](https://discord.gg/2NvYTcv)

# ThunderBolt Launcher

Кастомный лаунчер на базе Aurora Launcher для сервера ThunderBolt.

## 🚀 Быстрый старт

### Запуск сервера:
```bash
cd packages/server
npm install
npm run build:dev
node dist/LauncherServer.js
```

### Сборка клиента:
См. [ИНСТРУКЦИЯ_СБОРКИ_EXE.md](./ИНСТРУКЦИЯ_СБОРКИ_EXE.md)

## 📋 Настройка

- **Сервер:** `145.239.86.211:9274`
- **База данных:** MySQL (`s309042_REGISTRATION`)
- **Профиль:** `ThunderBolt` (Minecraft 1.20.1)

## 🔧 Конфигурация

- Файл сервера: `packages/server/dist/LauncherServerConfig.hjson`
- Файл клиента: `packages/launcher/config.ts`
- Профили: `packages/server/dist/profiles/`

## 📖 Документация

- [ИНСТРУКЦИЯ_СБОРКИ_EXE.md](./ИНСТРУКЦИЯ_СБОРКИ_EXE.md) - Как собрать .exe
- [ВСЕ_ВАРИАНТЫ_СБОРКИ_EXE.md](./ВСЕ_ВАРИАНТЫ_СБОРКИ_EXE.md) - Все способы сборки
- [README_SETUP.md](./README_SETUP.md) - Детальная настройка

## 🏗️ Сборка через GitHub Actions

1. Загрузите код на GitHub
2. Перейдите в Actions
3. Запустите workflow "Build Windows Launcher"
4. Скачайте готовый .exe из Artifacts

## 📝 Лицензия

MIT (базируется на Aurora Launcher)
