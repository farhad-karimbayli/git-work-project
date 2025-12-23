Цель: освоить базовый Git/GitHub workflow и стандартизировать коммиты через Conventional Commits.


Настроено:
- Conventional Commits
- commitlint
- husky (commit-msg hook)
- commitizen (коммиты через `npx cz`)


При 3 шаге с настройкой commitlint husky commitizen 
Получил:
npm WARN deprecated inflight@1.0.6
npm WARN deprecated glob@7.2.3
Пакет больше не поддерживается но ещё работает 

После добавления файла через git add commit-msg hook начал корректно отрабатывать и блокировать неверные сообщения коммитов.
