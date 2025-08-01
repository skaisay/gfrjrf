# Roblox Stats Tracker

Полноценное PWA приложение для отслеживания статистики игроков в Roblox с современным стеклянным дизайном в стиле iPhone.

## 🚀 Особенности

- **PWA (Progressive Web App)** - устанавливается как нативное приложение
- **Работа без интернета** - все данные хранятся локально
- **Стеклянный дизайн** - современный UI в стиле iOS с эффектами стекла
- **Адаптивный интерфейс** - оптимизирован для ПК, планшетов и мобильных устройств
- **Локальное хранение** - все данные остаются на вашем устройстве

## 📱 Функциональность

### Главная страница
- Обзор общей статистики
- Последняя активность
- Быстрый доступ к основным функциям

### Управление игроками
- Добавление новых игроков
- Редактирование существующих профилей
- Удаление игроков
- Загрузка скриншотов

### Детальная статистика
- Количество убийств
- Количество смертей  
- K/D соотношение
- Время игры
- Эффективность (убийств в час)
- Просмотр скриншотов

## 🛠️ Установка

### Вариант 1: Локальная установка

1. Скачайте все файлы проекта в папку
2. Откройте `index.html` в браузере
3. Нажмите на иконку "Установить приложение" в адресной строке браузера
4. Подтвердите установку

### Вариант 2: Через GitHub Pages

1. Загрузите файлы в репозиторий на GitHub
2. Включите GitHub Pages в настройках репозитория
3. Перейдите по ссылке GitHub Pages
4. Установите как PWA

### Вариант 3: Локальный сервер

```bash
# Если у вас установлен Python
python -m http.server 8000

# Если у вас установлен Node.js
npx serve .

# Затем откройте http://localhost:8000 в браузере
```

## 📁 Структура проекта

```
roblox-stats-tracker/
├── index.html          # Главная страница
├── styles.css          # Стили приложения
├── app.js              # Основная логика
├── manifest.json       # PWA манифест
├── sw.js               # Service Worker
├── offline.html        # Страница оффлайн режима
├── icons/              # Иконки приложения
│   └── icon.svg        # Базовая иконка
└── README.md           # Этот файл
```

## 🎨 Создание иконок

Для полноценной работы PWA необходимо создать иконки разных размеров из базового SVG файла:

### Требуемые размеры:
- 72x72px
- 96x96px  
- 128x128px
- 144x144px
- 152x152px
- 192x192px
- 384x384px
- 512x512px

### Инструменты для создания иконок:
- [PWA Builder](https://www.pwabuilder.com/) - автоматическая генерация
- [Real Favicon Generator](https://realfavicongenerator.net/) - ручная настройка
- Любой графический редактор (Photoshop, GIMP, Figma)

## 🔧 Настройка фонов

Приложение поддерживает кастомные фоны. Измените CSS переменные в `styles.css`:

```css
body {
    background: linear-gradient(135deg, #ваш-цвет-1 0%, #ваш-цвет-2 100%);
    /* или используйте изображение */
    background: url('path/to/your/background.jpg') center/cover;
}
```

## 💾 Данные и резервное копирование

- Все данные автоматически сохраняются в localStorage браузера
- Данные сохраняются даже при закрытии браузера
- Для резервного копирования можно добавить функции экспорта/импорта
- Данные привязаны к домену, на котором работает приложение

## 🌐 Браузерная поддержка

- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Все современные мобильные браузеры

## 📝 Использование

1. **Добавление игрока**: 
   - Перейдите на вкладку "Игроки"
   - Нажмите "Добавить игрока"
   - Заполните форму и сохраните

2. **Редактирование статистики**:
   - Нажмите на иконку редактирования у нужного игрока
   - Обновите данные
   - Сохраните изменения

3. **Просмотр детальной статистики**:
   - Перейдите на вкладку "Статистика"
   - Выберите игрока из списка
   - Просмотрите подробную информацию

4. **Загрузка скриншотов**:
   - При создании/редактировании игрока
   - Выберите файл изображения
   - Скриншот будет сохранен локально

## 🔐 Безопасность и приватность

- Все данные хранятся локально на вашем устройстве
- Никакие данные не передаются на внешние серверы
- Приложение работает полностью автономно
- Для очистки данных используйте настройки браузера

## 🎯 Планы развития

- [ ] Экспорт/импорт данных
- [ ] Темная/светлая тема
- [ ] Графики и диаграммы
- [ ] Сравнение игроков
- [ ] Push-уведомления
- [ ] Синхронизация между устройствами (опционально)

## 🐛 Известные проблемы

- В некоторых старых браузерах могут не работать эффекты стекла
- На iOS Safari может потребоваться двойное нажатие для установки PWA

## 📄 Лицензия

MIT License - используйте свободно для личных и коммерческих проектов.

## 🤝 Поддержка

Если у вас возникли вопросы или проблемы:
1. Проверьте консоль браузера на наличие ошибок
2. Убедитесь, что все файлы загружены корректно
3. Попробуйте очистить кэш браузера
4. Проверьте, что браузер поддерживает PWA

---

**Создано с ❤️ для сообщества Roblox игроков**
