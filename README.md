Интернет-магазин API API для интернет-магазина, разработанный с использованием фреймворка Laravel.

Установка Склонируйте репозиторий на вашу локальную машину: git clone https://github.com/your-username/your-repository.git Перейдите в директорию проекта: cd your-repository Установите зависимости через Composer: composer install Создайте файл .env на основе .env.example и настройте подключение к базе данных: cp .env.example .env Сгенерируйте ключ приложения: php artisan key:generate Выполните миграции для создания таблиц базы данных: Copy code php artisan migrate Запустите встроенный сервер разработки: Copy code php artisan serve Приложение будет доступно по адресу http://localhost:8000. Использование Для регистрации нового пользователя отправьте POST-запрос на /api/register с JSON-телом, содержащим имя пользователя, адрес электронной почты и пароль.

Для аутентификации пользователя отправьте POST-запрос на /api/login с JSON-телом, содержащим адрес электронной почты и пароль.

Для получения списка категорий в виде дерева отправьте GET-запрос на /api/categories.

Для получения списка продуктов с фильтрацией отправьте GET-запрос на /api/products с параметрами фильтрации.

Для добавления продукта в корзину отправьте POST-запрос на /api/cart с JSON-телом, содержащим идентификатор продукта и количество.

Для редактирования количества продукта в корзине отправьте PUT-запрос на /api/cart/{cartId} с JSON-телом, содержащим новое количество.

Для удаления продукта из корзины отправьте DELETE-запрос на /api/cart/{cartId}.

Для оформления заказа отправьте POST-запрос на /api/order с JSON-телом, содержащим контактные данные и список выбранных продуктов.

Для получения списка оформленных заказов отправьте GET-запрос на /api/orders.

Документация API Дополнительная документация по API, включая список доступных эндпоинтов и параметры запросов, доступна в Postman коллекции
