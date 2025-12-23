Отчёт: Git/GitHub 

Что было сделно
1. Создал публичный репозиторий и склонировал его локально.
2. Работал через feature-ветку `feature/commit-setup` без прямых коммитов в main.
3. Настроил commitlint, husky (commit-msg hook) и commitizen.
4. Все коммиты создавались через `npx cz` в формате Conventional Commits.
5. Открыл Pull Request и внёс правки новыми коммитами после комментариев.
6. Смёржил Pull Request в main.

Что настроено и где:

commitlint
- Файл: `commitlint.config.cjs`
- Использован `@commitlint/config-conventional`
- Ограничены типы коммитов: feat, fix, chore, refactor, docs

husky
- Инициализация через `npm run prepare`
- Hook: `.husky/commit-msg`
- Проверка сообщений коммитов через commitlint

commitizen
- Коммиты создавались через `npx cz`

## Доказательства
- Pull Request: <ССЫЛКА НА PR>
- Пример истории:
```bash
git log --oneline
