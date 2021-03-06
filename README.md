Git trunk-based-development patterns <sup>8 ак.ч.</sup>
====================================

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
- [detached head](http://pr0git.blogspot.com/2015/03/git.html) state
- [ ] Debrief

Обзор workflow в git <sup>0.5</sup>
--------------------
- [ ] [Что это?](https://ndpsoftware.com/git-cheatsheet.html)
- [ ] Live coding session
- checkout to working dir
- implicit "tags" = refs
- [`soft reset`](https://stackoverflow.com/a/5201642) для squash и расщепления коммита (soft reset + частичный коммит + частичный коммит)
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

Сценарий: `squash` <sup>0.5</sup>
------------------
- [ ] [Зачем это?](https://softwareengineering.stackexchange.com/questions/263164/why-squash-git-commits-for-pull-requests)
- [как?](https://www.jetbrains.com/help/idea/edit-project-history.html#squash-commits)
- [`soft reset`](https://stackoverflow.com/a/5201642)
- [ ] Live coding session
- [ ] Practice session
- [ ] Debrief

Сценарий: `rebase` <sup>1</sup>
------------------
- [ ] Что это?
- [ ] Зачем?
- [ ] Как можно слить ветки
- `fast-forward`
- [merge](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging#_basic_merging)
- [rebase](https://git-scm.com/book/en/v2/Git-Branching-Rebasing) 
- + `fast-forward` merge
- + [3-arguments surgery](https://qastack.ru/programming/29914052/i-cant-understand-the-behaviour-of-git-rebase-onto)
- [ ] [merge vs rebase](https://www.atlassian.com/ru/git/tutorials/merging-vs-rebasing)
- [ ] Live coding session
- [Rebase with IDEA](https://www.jetbrains.com/help/idea/apply-changes-from-one-branch-to-another.html#rebase-branch)
- [Interactive rebase with IDEA](https://www.jetbrains.com/help/idea/edit-project-history.html)
- [ ] Practice session
- [ ] Debrief

Сценарий: как найти потерянные коммиты в истории <sup>0.5</sup>
------------------------------------------------
- [ ] [Подвисшие/потерянные коммиты и blob](https://stackoverflow.com/questions/18514659/git-what-is-a-dangling-commit-blob-and-where-do-they-come-from)
- [git gc](https://www.atlassian.com/git/tutorials/git-gc)
- [как найти](https://stackoverflow.com/questions/10099258/how-can-i-recover-a-lost-commit-in-git) и [починить просто](https://www.ocpsoft.org/tutorials/git/use-reflog-and-cherry-pick-to-restore-lost-commits/)
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
- [ ] Что это?
- [ ] Зачем?
- [ ] [Как? (для github)](https://medium.com/sweetmeat/how-to-keep-a-downstream-git-repository-current-with-upstream-repository-changes-10b76fad6d97)
- [ ] Practice session
- [ ] Debrief

Процесс: `trunk-based development`, `TBD` <sup>0.5</sup>
-----------------------------------------
- [ ] [Что это?](https://trunkbaseddevelopment.com)
- [`branch by abstraction`](https://www.branchbyabstraction.com) `technique to counter the pressure to create a long-lived branch that would merge “back” later`
- [`feature toggling`](https://martinfowler.com/articles/feature-toggles.html)
- [ ] [Зачем?](https://habr.com/ru/post/519314/)
- [ ] [Но это же больно?](https://martinfowler.com/bliki/FrequencyReducesDifficulty.html)
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
