# Пример микрофронтенд-архитектуры на Vue 3 и Vite

Этот репозиторий демонстрирует реализацию **микрофронтенд-архитектуры** с использованием Vue 3, Vite и Module Federation. Каждый микрофронтенд работает в изолированном экземпляре Vue, что обеспечивает независимость модулей и гибкость разработки.

## Функционал

- **Микрофронтенды**: Независимые модули с отдельными экземплярами Vue.
- **Динамическая загрузка**: Использование Webpack Module Federation.
- **Управление маршрутами**: Манифест маршрутов (`Route Manifest`) для динамической регистрации путей.
- **Монорепозиторий**: Управление проектом через Lerna и NPM Workspaces.
- **Оптимизация**: Vite для быстрой сборки и горячей перезагрузки (HMR).

## Структура проекта

```sh
micro-frontend-sample/
├── packages/
│   ├── host/          # Shell application (Main container)
│   ├── app-1/         # Micro frontend 1
│   ├── app-2/         # Micro frontend 2
│
├── package.json       # Monorepo package manager with workspaces
├── lerna.json         # Lerna configuration
├── README.md          # Documentation
```

## Установка и запуск

### Клонирование репозитория

```sh
git git@github.com:vkrysin/micro-frontend-test.git
cd micro-frontend-test
```

### Установка зависимостей

Используя npm:

```sh
npm i -r
```

### Запуск приложений

Запуск всех приложений:

```sh
npm run dev
```

## Доступ к приложениям

| Micro Frontend | URL                     |
| -------------- | ----------------------- |
| Host App       | `http://localhost:5010` |
| App 1          | `http://localhost:5011` |
| App 2          | `http://localhost:5012` |

