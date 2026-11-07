# Как запустить проект Angular-HelloWorld
# Репозиторий: https://github.com/DanWahlin/Angular-HelloWorld

# ПРЕДУСЛОВИЯ 
# Нужны: git, Node.js LTS, npm. Порт 4200 свободен.
# Angular CLI глобально ставить НЕ обязательно (используем npx).

# Шаг 1. Проверка окружения 
node -v
npm -v
git --version

# Шаг 2. Клонирование проекта 
git clone https://github.com/DanWahlin/Angular-HelloWorld.git
cd Angular-HelloWorld

# Шаг 3. Установка зависимостей 
npm install

# Шаг 4. Запуск dev-сервера 
# Это блокирующая команда, остановить: Ctrl+C
# После запуска откройте в браузере: http://localhost:4200/
npx ng serve --open

# Шаг 5. Сборка проекта 
# Сначала остановите dev-сервер (Ctrl+C), потом выполните:
npx ng build
# Результат появится в папке dist/

# Шаг 6. Юнит-тесты 
# Остановить: Ctrl+C
npx ng test

# Шаг 7. E2E-тесты 
# Работает только если в проекте уже настроен e2e-пакет
npx ng e2e

# Шаг 8. Генерация нового компонента (пример) 
npx ng generate component component-name


# РЕЗУЛЬТАТ
# После `npx ng serve --open` приложение откроется
# в браузере на http://localhost:4200/
# При изменении файлов в src/ страница перезагрузится сама.
#
# После `npx ng build` готовые файлы будут в dist/.
#
# Если Angular CLI уже стоит глобально,
# можно заменить `npx ng ...` на `ng ...`.