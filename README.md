# 📝 TODO приложение (Pet Project)

## Описание проекта

В этом проекте вы реализуете простое консольное приложение для управления списком задач (TODO list).  
Это поможет закрепить навыки **ООП в Java**, работу с **Collections API**, **Streams**, обработку ошибок и написание **юнит-тестов**.

Проект имитирует реальную работу над “продакшн‑кодом”:
- Разделение на слои (Controller → Service → Repository)
- Чёткая бизнес‑логика
- Тестирование

---

## Цели проекта

- Научиться писать **читаемый, структурированный код**
- Освоить слоистую архитектуру приложений
- Закрепить навыки работы с:
    - **Коллекциями (List, Map)**
    - **Streams API**
    - **Enum и исключениями**
- Практиковаться в написании **юнит‑тестов (JUnit)**

---

## Технологический стек

- ✅ **Java 17+**
- ✅ **Collections + Streams API**
- ✅ **JUnit** — для тестов
- ✅ **Lombok** — для сокращения шаблонного кода
- ✅ **Gradle** (приоритет) или Maven — система сборки
- ✅ **Git** — для контроля версий

---

## Функционал приложения

Пользователь может:

- Просматривать список всех задач
- Добавить задачу с:
  - Названием
  - Описанием
  - Сроком выполнения (LocalDate)
- Редактировать задачу:
  - Изменить название, описание, срок
  - Изменить статус (TODO / IN_PROGRESS / DONE)
- Удалить задачу
- Фильтровать задачи по статусу
- Сортировать задачи по:
  - сроку выполнения
  - статусу

---

## Команды в консоли

| Команда   | Описание                              |
|-----------|---------------------------------------|
| `add`     | Добавить новую задачу                 |
| `list`    | Показать все задачи                   |
| `edit`    | Редактировать существующую задачу     |
| `delete`  | Удалить задачу                        |
| `filter`  | Показать задачи с определённым статусом|
| `sort`    | Отсортировать задачи                  |
| `exit`    | Завершить работу приложения           |

---

## Архитектура

### Controller
- Принимает команды пользователя
- Вызывает методы сервиса
- Отвечает за взаимодействие с пользователем

### Service
- Содержит бизнес-логику:
  - Добавление задач
  - Редактирование
  - Фильтрация и сортировка
- Вызывает репозиторий для доступа к данным

### Repository
- Хранит задачи в **коллекции**
- Предоставляет методы для CRUD операций

---

## Тестирование

- Написать **юнит‑тесты** для методов `TaskService` с использованием JUnit, Mockito
- Протестировать:
  - Добавление задачи
  - Редактирование
  - Удаление
  - Фильтрацию и сортировку

❗ Тесты для контроллера и репозитория **НЕ требуются**

---

## Требования

- Java 17+
- Gradle (предпочтительно) или Maven
- Зависимости:
  - Lombok
  - JUnit

---

## Советы
- Делайте код **читаемым**: используйте понятные имена методов и переменных
- Обрабатывайте ошибки красиво (например, при попытке удалить несуществующую задачу)
- Не бойтесь рефакторить код — это нормально на этом этапе

---

## Результат

После завершения проекта вы получите:

✅ Консольное TODO-приложение  
✅ Навыки написания бизнес-логики  
✅ Опыт работы с Collections и Streams  
✅ Опыт написания юнит‑тестов 