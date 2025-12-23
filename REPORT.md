Цель: освоить базовый Git/GitHub workflow и стандартизировать коммиты через Conventional Commits.


Настроено:
- Conventional Commits
- commitlint
- husky (commit-msg hook)
- commitizen (коммиты через `npx cz`)


Step 3 шаге с настройкой commitlint husky commitizen
Получил:
npm WARN deprecated inflight@1.0.6
npm WARN deprecated glob@7.2.3
Пакет больше не поддерживается но ещё работает

После добавления файла через `git add` commit-msg hook начал корректно отрабатывать и блокировать неверные сообщения коммитов.
Пока это работает не правильно в процессе исправления
Исправленно в Husky команда `husky add` устарела
Commit-msg hook был создан вручную в директории `.husky`
путь к hooks явно указан через `git config core.hooksPath .husky`
Это позволило корректно подключить commitlint и блокировать некорректные сообщения коммитов

Step 4 Branches and Commits
Working successfully


Что сделано
- Настроены commitlint и husky commit-msg hook для проверки сообщений коммитов
- Подключён commitizen все коммиты создаются через `npx cz`
- Добавлены contributing guidelines


Зачем это нужно
- Единый формат сообщений коммитов делает работу с проектом удобной и читаемой историю
- Husky и commitlint автоматически блокируют некорректные сообщения коммитов


Проверка работоспособности
- Сделать коммит через `npx cz`  коммит должен пройти
- Попробовать `git commit -m "bad message"`  коммит должен быть заблокирован

Для корректной работы Git hooks путь к хукам был явно указан командой `git config core.hooksPath .husky`


All working correctly 