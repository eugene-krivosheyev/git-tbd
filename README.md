Git trunk-based-development patterns <sup>8 ак.ч.</sup>
====================================

Записи
------
- [26.07](https://us02web.zoom.us/rec/share/Qz0EWQA_hIoNCpP2e70MZ0E2_G31MiAusi0kM0ADA4c1uoyzRikmfz_YA54K2NZ9.ejv_nkvZMEcLXafy)
- [27.07](https://us02web.zoom.us/rec/share/rgelW7cuVurqX2MHYsTNl-NBRqYEHFOXZZ_NWcWMpyjuL4C_0eJm_12zqG4ytJOq.uriRHjsqNcbdPS1X)
- [28.07](https://us02web.zoom.us/rec/share/LpLc3UN7lrx5bm_g9k7C54AQi9ykLZM7wsmW8l_f5K4qfCt3QG5TLW8nIf5Bnhgy.DiZALyd_gW48Epev)

Введение <sup>0.5</sup>
--------
- [ ] Тренер и контакты
- [ ] Метафора курса
- [ ] Договоренности (вопросы, перерывы, записи)
- [ ] Обзор тем
- [ ] Участники (роль, уровень, проблемы)
- amend, cherry pick, squash, rebase
- [ ] Почему сегодня важны практики CM и куда мы двигаемся

Обзор git client в IDEA <sup>0.5</sup>
-----------------------
- [ ] Что это?
- [ ] Зачем?
- [ ] Live coding session
- настройки
- git stage vs idea shelve
- базовые операции: меню и git view
- hotkeys
- [ ] Practice session
- [ ] Debrief

Обзор workflow в git <sup>0.5</sup>
--------------------
- [ ] [Что это?](https://ndpsoftware.com/git-cheatsheet.html)
- [ ] Live coding session
- checkout to working dir
- implicit "tags" / refs
- [ ] Practice session
- [паттерны переключения между задачами](https://www.jetbrains.com/help/idea/work-on-several-features-simultaneously.html)
- [ ] Debrief

Сценарий: `conventional commits` + `semantic versioning tags` <sup>0.5</sup>
-------------------------------------------------------------
- [ ] Что это?
- [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [semantic versioning tags](https://semver.org)
- [ ] Зачем?
- [ ] Practice session
- [ ] Debrief

Сценарий: `cherry pick` <sup>0.5</sup>
-----------------------
- [ ] [Что это?](https://git-scm.com/book/ru/v2/Распределенный-Git-Сопровождение-проекта#r_rebase_cherry_pick)
- [ ] [Зачем?](https://www.atlassian.com/git/tutorials/cherry-pick)
- [ ] Live coding session
- [ ] Practice session
- [ ] Debrief

Сценарий: `rebase` <sup>1</sup>
------------------
- [ ] Что это?
- [ ] Зачем?
- [merge](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging#_basic_merging) + ff
- [rebase](https://git-scm.com/book/en/v2/Git-Branching-Rebasing) + `fast-forward` merge
- [merge vs rebase](https://www.atlassian.com/ru/git/tutorials/merging-vs-rebasing)
- [ ] Live coding session
- [modifying branch history with IDEA](https://www.jetbrains.com/help/idea/edit-project-history.html)
- [ ] Practice session
- [ ] Debrief

Сценарий: `squash` <sup>0.5</sup>
------------------
- [ ] [Что это?](https://ru.stackoverflow.com/questions/433993/Как-работает-git-merge-squash)
- [`soft reset`](https://stackoverflow.com/a/5189600)
- [ ] Зачем?
- [ ] Live coding session
- [ ] Practice session
- [ ] Debrief

Сценарий: как найти потерянные коммиты в истории <sup>0.5</sup>
------------------------------------------------
- [ ] [Подвисшие/потерянные коммиты и blob](https://stackoverflow.com/questions/18514659/git-what-is-a-dangling-commit-blob-and-where-do-they-come-from)
- [git gc](https://www.atlassian.com/git/tutorials/git-gc)
- [как найти](https://stackoverflow.com/questions/10099258/how-can-i-recover-a-lost-commit-in-git)
- [указатели ссылок](https://stackoverflow.com/questions/26785118/head-vs-head-vs-head-also-known-as-tilde-vs-caret-vs-at-sign) и `git help revisions`
- [ ] Live coding session
- [ ] Practice session
- [ ] Debrief

Процесс: обзор моделей ветвления <sup>0.5</sup>
--------------------------------
- [ ] [Что это?](https://medium.com/@patrickporto/4-branching-workflows-for-git-30d0aaee7bf)
- [ ] Зачем?
- [ ] Practice session
- [ ] Debrief

Процесс: `regular downstream sync` <sup>0.5</sup>
----------------------------------
- [ ] [Что это?](https://www.atlassian.com/git/tutorials/git-forks-and-upstreams)
- [ ] Зачем?
- [ ] Practice session
- [ ] Debrief

Процесс: `trunk-based development`, `TBD` <sup>0.5</sup>
-----------------------------------------
- [ ] [Что это?](https://trunkbaseddevelopment.com)
- [`branch by abstraction`](https://martinfowler.com/bliki/BranchByAbstraction.html)
- [`feature toggling`]()
- [ ] [Зачем?](https://habr.com/ru/post/519314/)
- [ ] Practice session
- [ ] Debrief

Процесс: целевая архитектура voximplant CM <sup>0.5</sup>
------------------------------------------
- [ ] Как выглядит наша целевая CM архитектура
- epic feature: dev -> epic branch -> feature branch -> epic branch (squash + rebase) -> trunk (ff или rebase)
- fast feature: dev -> feature branch -> dev (ff или rebase)
- hot fix: trunk -> hot fix branch -> trunk (squash + rebase) + dev (cherry pick)
- [ ] Почему именно так?
- [ ] Кейс «зависимые задачи, но первая еще не влита»
- [ ] Practice session
- [ ] Debrief

Ретро <sup>0.5</sup>
-----
- [ ] Оставшиеся вопросы и запаркованные темы
- [ ] Коммитмент на конкретные действия на производстве

Беклог
------
- [ ] detached head
- [ ] git blame
- [ ] push --force отличается от push --force-with-lease
- [ ] "оффлайн-хуки"
- [ ] ветки, которые не берут начало из другой ветки, кроме мастера

