CONTRIBUTING.md

English

---

Contributing to BTG

First of all, thank you for considering contributing to BTG. We appreciate your time and effort.

---

What we expect

Before you start writing code, please understand our philosophy. BTG is not just another collection of utilities. It is an engineering standard.

Every contribution must follow the three pillars of BTG:

1. Lightweight and Fast. Startup under 2 seconds, minimal memory usage, native languages only.
2. Stable. No crashes, no system breaking, all edge cases handled gracefully.
3. Modular. Every feature can be disabled or removed without breaking the core.

If your code violates any of these principles, it will not be accepted.

---

How to contribute

1. Find an issue.

Check the Issues page. Look for labels like "good first issue" or "help wanted".

If you want to add a new utility, open an issue first to discuss it. We do not want you to waste your time on something we might reject.

1. Fork and clone.

```
git clone https://github.com/yourname/btg.git
cd btg
```

1. Create a branch.

```
git checkout -b feature/your-feature-name
```

1. Write code.

Follow these rules:

· Use C, Rust, Go or Zig. No Python, JavaScript, Ruby or other interpreted languages.
· Keep dependencies minimal. No more than 3 indirect dependencies.
· Write comments in English.
· Keep functions small and focused.
· Add tests for every new feature.

1. Test your code.

```
make test
```

All tests must pass. No exceptions.

1. Update documentation.

· Update README.md if you added or changed a utility.
· Update UTILITIES.md with your utility description.
· Add comments to your code.
· If your utility has flags, document them in --help.

1. Commit.

Write clear commit messages:

```
btg-ls: add color output support

Adds --color flag to enable colored output.
Closes #42
```

1. Push and create a Pull Request.

Push your branch and open a Pull Request against main.

Describe your changes clearly. Link the issue you are solving.

---

Code style

C language

· Follow K&R style
· Use snake_case for functions and variables
· Use UPPER_CASE for constants
· Indent with 4 spaces

Rust language

· Follow standard Rust style (cargo fmt)
· Use snake_case for functions and variables
· Use CamelCase for types

Go language

· Follow standard Go style (go fmt)
· Use camelCase for private, PascalCase for public

Zig language

· Follow standard Zig style
· Use snake_case for functions and variables

---

Testing requirements

Every utility must have:

· Unit tests for each function
· Integration tests for user-facing commands
· Edge case tests (empty input, huge files, invalid arguments)

Test coverage should be at least 80 percent.

---

Performance requirements

· Startup time must be measured and documented
· Memory usage must be measured and documented
· No memory leaks (use valgrind or similar tools)
· No unnecessary allocations

---

Documentation requirements

· Every utility must have --help output
· Every utility must have a man page (or at least a README section)
· Every public function must have a comment
· Every module must have a comment explaining its purpose

---

What not to do

· Do not copy code from GNU or other projects
· Do not add unnecessary dependencies
· Do not break existing API without a very good reason
· Do not ignore code reviews
· Do not submit large pull requests without prior discussion

---

Review process

1. A maintainer will review your Pull Request within 48 hours.
2. They will test your code manually.
3. They may ask for changes.
4. Once approved, your code will be merged.

We are strict but fair. Do not take comments personally. We all want BTG to be great.

---

Recognition

Every contributor will be listed in CONTRIBUTORS.md. We value your work.

---

Questions

Open an issue.

---

Thank you for making BTG better.

---

---

Русский

---

Вклад в проект BTG

Прежде всего, спасибо, что решили помочь BTG. Мы ценим ваше время и усилия.

---

Что мы ожидаем

Прежде чем писать код, пожалуйста, ознакомьтесь с нашей философией. BTG это не просто очередной набор утилит. Это инженерный стандарт.

Каждый вклад должен соответствовать трём столпам BTG:

1. Лёгкость и быстрота. Запуск до 2 секунд, минимальное потребление памяти, только нативные языки.
2. Стабильность. Никаких падений, никаких поломок системы, все краевые случаи обработаны корректно.
3. Модульность. Каждая функция может быть отключена или удалена без потери базовой функциональности.

Если ваш код нарушает любой из этих принципов, он не будет принят.

---

Как внести вклад

1. Найдите задачу.

Посмотрите страницу Issues. Ищите метки "good first issue" или "help wanted".

Если вы хотите добавить новую утилиту, сначала откройте обсуждение. Мы не хотим, чтобы вы тратили время на то, что мы можем отклонить.

1. Сделайте форк и клонируйте.

```
git clone https://github.com/yourname/btg.git
cd btg
```

1. Создайте ветку.

```
git checkout -b feature/название-вашей-функции
```

1. Пишите код.

Следуйте правилам:

· Используйте C, Rust, Go или Zig. Никаких Python, JavaScript, Ruby или других интерпретируемых языков.
· Минимум зависимостей. Не более 3 косвенных зависимостей.
· Пишите комментарии на английском.
· Держите функции маленькими и сфокусированными.
· Добавляйте тесты для каждой новой функции.

1. Протестируйте код.

```
make test
```

Все тесты должны проходить. Без исключений.

1. Обновите документацию.

· Обновите README.md, если добавили или изменили утилиту.
· Обновите UTILITIES.md с описанием вашей утилиты.
· Добавьте комментарии к коду.
· Если у вашей утилиты есть флаги, опишите их в --help.

1. Сделайте коммит.

Пишите понятные сообщения коммитов:

```
btg-ls: добавить поддержку цветного вывода

Добавляет флаг --color для включения цветного вывода.
Закрывает #42
```

1. Отправьте изменения и создайте Pull Request.

Отправьте ветку и откройте Pull Request в ветку main.

Опишите ваши изменения понятно. Ссылайтесь на задачу, которую вы решаете.

---

Стиль кода

Язык C

· Стиль K&R
· snake_case для функций и переменных
· UPPER_CASE для констант
· Отступы 4 пробела

Язык Rust

· Стандартный стиль Rust (cargo fmt)
· snake_case для функций и переменных
· CamelCase для типов

Язык Go

· Стандартный стиль Go (go fmt)
· camelCase для приватных, PascalCase для публичных

Язык Zig

· Стандартный стиль Zig
· snake_case для функций и переменных

---

Требования к тестированию

Каждая утилита должна иметь:

· Модульные тесты для каждой функции
· Интеграционные тесты для пользовательских команд
· Тесты краевых случаев (пустой ввод, огромные файлы, неверные аргументы)

Покрытие тестами должно быть не менее 80 процентов.

---

Требования к производительности

· Время запуска должно быть измерено и задокументировано
· Потребление памяти должно быть измерено и задокументировано
· Нет утечек памяти (используйте valgrind или аналоги)
· Нет лишних аллокаций

---

Требования к документации

· У каждой утилиты должен быть вывод --help
· У каждой утилиты должна быть man-страница (или хотя бы секция в README)
· У каждой публичной функции должен быть комментарий
· У каждого модуля должен быть комментарий с описанием назначения

---

Чего не делать

· Не копируйте код из GNU или других проектов
· Не добавляйте лишние зависимости
· Не ломайте существующий API без веской причины
· Не игнорируйте ревью кода
· Не отправляйте большие пул-реквесты без предварительного обсуждения

---

Процесс ревью

1. Мейнтейнер рассмотрит ваш Pull Request в течение 48 часов.
2. Он протестирует ваш код вручную.
3. Возможно, попросит внести изменения.
4. После одобрения ваш код будет влит.

Мы строгие, но справедливые. Не воспринимайте комментарии лично. Мы все хотим, чтобы BTG был отличным.

---

Благодарность

Каждый контрибьютор будет добавлен в CONTRIBUTORS.md. Мы ценим вашу работу.

---

Вопросы

Откройте задачу.

---

Спасибо, что делаете BTG лучше.
