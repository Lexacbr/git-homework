# Домашнее задание к занятию "`Git" - `Савельев Алексей SYS-25`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw.
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1

1. У меня был уже зарегистророван аккаунт, поэтому этот этап пропущу
2. Клонирую задание  себе на компьютер
```bash
sav@sav-Lenovo-G580:~$ git clone https://github.com/Lexacbr/git-homework
Клонирование в «git-homework»...
remote: Enumerating objects: 73, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 73 (delta 0), reused 0 (delta 0), pack-reused 70
Получение объектов: 100% (73/73), 3.58 МиБ | 1.83 МиБ/с, готово.
Определение изменений: 100% (27/27), готово.
```
![Скриншот терминала](https://github.com/Lexacbr/git-homework/blob/main/img/scr_sh.png)

4. Указал своё имя и почту
```bash
sav@sav-Lenovo-G580:~$ git config --global user.name savelev.aleksey
sav@sav-Lenovo-G580:~$ git config --global user.email aleksej05@mail.ru
```
5. Выполнил команду:
```bash
sav@sav-Lenovo-G580:~$ git status
Текущая ветка: main
Неотслеживаемые файлы:
(используйте «git add <файл>...», чтобы добавить в то, что будет включено в коммит)
индекс пуст, но есть неотслеживаемые файлы
(используйте «git add», чтобы проиндексировать их)
```
6. Редактировал файл в Visual Studio Code

![vscode](https://github.com/Lexacbr/git-homework/blob/main/img/vscode.png)

7. Вывод команды git status 
```bash
sav@sav-Lenovo-G580:~/git-homework$ git status
Текущая ветка: main
Эта ветка соответствует «origin/main».

Неотслеживаемые файлы:
  (используйте «git add <файл>...», чтобы добавить в то, что будет включено в коммит)
        img/vscode.png

индекс пуст, но есть неотслеживаемые файлы
(используйте «git add», чтобы проиндексировать их)
```
8. Выполнил команды: `git diff` и `diff --staged`  У команды `git diff`  был слишком подробный вывод и сюда прикреплять я его не стал
```bash
sav@sav-Lenovo-G580:~/git-homework$ git diff --staged
diff --git a/img/vscode.png b/img/vscode.png
new file mode 100644
index 0000000..80e8494
Binary files /dev/null and b/img/vscode.png differ
sav@sav-Lenovo-G580:~/git-homework$ 
```
9. Всё "запушил".

[Ссылка на коммит](https://github.com/netology-code/sys-pattern-homework/commit/9b9eff5ab279cbe81d0cbc910b7dee71a42f1525)

---

### Задание 2

1. Создал файл `./gitignore` из меню VSCode
2. Добавил файл в ветку
```bash
sav@sav-Lenovo-G580:~/git-homework$ git add .gitignore
sav@sav-Lenovo-G580:~/git-homework$ git status
Текущая ветка: main
Ваша ветка опережает «origin/main» на 1 коммит.
  (используйте «git push», чтобы опубликовать ваши локальные коммиты)

Изменения, которые будут включены в коммит:
  (используйте «git restore --staged <файл>...», чтобы убрать из индекса)
        новый файл:    .gitignore

```
3. Сразу запушил
```bash
sav@sav-Lenovo-G580:~/git-homework$ git push 
Перечисление объектов: 5, готово.
Подсчет объектов: 100% (5/5), готово.
При сжатии изменений используется до 4 потоков
Сжатие объектов: 100% (3/3), готово.
Запись объектов: 100% (3/3), 631 байт | 631.00 КиБ/с, готово.
Всего 3 (изменений 1), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lexacbr/git-homework
   277cf1d..173ee97  main -> main
```
4. Прописал правила игнорирования

![Ignore](https://github.com/Lexacbr/git-homework/blob/main/img/ignore.png)

5. Делаю коммит и пуш

[Ссылка на коммит](https://github.com/Lexacbr/git-homework/commit/cce8eb3bcf96b6229126839a2a0c86fd47c40b4b)

---

### Задание 3

1. Создаю ветку  dev и имитирую работу
2. Всё сделал по инструкции и получил вот такой результат: 

[Ссылка на Graph](https://github.com/Lexacbr/git-homework/network)

[Ссылка на все коммиты](https://github.com/Lexacbr/git-homework/commits/main)
 
 ---


