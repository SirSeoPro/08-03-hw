# Домашнее задание к занятию "`Git`" - `Кощеев Иван`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
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
Что нужно сделать:

1. Зарегистрируйте аккаунт на GitHub.

<details>

![image1](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_160426.png)

</details>

2. Создайте новый отдельный публичный репозиторий. Обязательно поставьте галочку в поле «Initialize this repository with a README».

<details>

![image2](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_171856.png)

</details>

3. Склонируйте репозиторий, используя https протокол git clone ....

<details>

![image3](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_172245.png)

</details>


4. Перейдите в каталог с клоном репозитория.

<details>

![image3](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_172404.png)

</details>

5. Произведите первоначальную настройку Git, указав своё настоящее имя и email: git config --global user.name и git config --global user.email johndoe@example.com.

<details>

```
git config --global ivon
git config --global user.email sir.seopro@gmail.com
```

</details>

6. Выполните команду git status и запомните результат.
7. Отредактируйте файл README.md любым удобным способом, переведя файл в состояние Modified.
8. Ещё раз выполните git status и продолжайте проверять вывод этой команды после каждого следующего шага.
9. Посмотрите изменения в файле README.md, выполнив команды git diff и git diff --staged.
10. Переведите файл в состояние staged или, как говорят, добавьте файл в коммит, командой git add README.md.
11. Ещё раз выполните команды git diff и git diff --staged.
12. Теперь можно сделать коммит git commit -m 'First commit'.

<details>

![image4](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_172823.png)

</details>

13. Сделайте git push origin master.

<details>

![image4](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_173118.png)

</details>

14. В качестве ответа добавьте ссылку на этот коммит в ваш md-файл с решением.

[Ссылка](https://github.com/SirSeoPro/git-08-01)


---

### Задание 2

1. Создайте файл .gitignore (обратите внимание на точку в начале файла) и проверьте его статус сразу после создания.
2. Добавьте файл .gitignore в следующий коммит git add....
3. Напишите правила в этом файле, чтобы игнорировать любые файлы .pyc, а также все файлы в директории cache.
4. Сделайте коммит и пуш.

<details>

![image5](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_174638.png)

</details>

[Ссылка](https://github.com/SirSeoPro/git-08-01/blob/main/.gitignore)
---

### Задание 3

1. Создайте новую ветку dev и переключитесь на неё.

<details>

```
ivon@ivon-VBox:~/projects/git_1001_2/git-08-01$ git checkout -b dev
Переключились на новую ветку «dev»
ivon@ivon-VBox:~/projects/git_1001_2/git-08-01$ git branch
* dev
  main

```

</details>

2. Создайте в ветке dev файл test.sh с произвольным содержимым.
3. Сделайте несколько коммитов и пушей в ветку dev, имитируя активную работу над файлом в процессе разработки.
4. Переключитесь на основную ветку.
5. Добавьте файл main.sh в основной ветке с произвольным содержимым, сделайте комит и пуш . Так имитируется продолжение общекомандной разработки в основной ветке во время разработки отдельного функционала в dev ветке.

<details>

![image6](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_175923.png)

</details>

6. Сделайте мердж dev ветки в основную с помощью git merge dev. Напишите осмысленное сообщение в появившееся окно комита.

<details>

![image7](https://github.com/SirSeoPro/08-03-hw/blob/main/screenshoots/Screenshot_20250110_180509.png)

</details>

7. Сделайте пуш в основной ветке.
8. Не удаляйте ветку dev.

[Ссылка](https://github.com/SirSeoPro/git-08-01/network)

