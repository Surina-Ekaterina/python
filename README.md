# PYTHON 2023
Рад всех приветствовать на курсе, посвященном программированию на языке Python!
Ниже вы найдете инструкцию по работе с GitHub.

# Начало работы
1. Зарегистрируйтесь в Git, используя вашу корпоративную почту: [GitHub](https://github.com/)
2. Скачайте и установите Git Bash: [Git for PC](https://git-scm.com/downloads)
3. Залогиньтесь в Git Bash. Инструкция [здесь](https://kbroman.org/github_tutorial/pages/first_time.html)
4. Создайте на вашем ПК папку, в которой будете хранить файлы курса. Это ваш локальный репозиторий.
5. Скопируйте файлы из моего репозитория к себе в папку. Для этого нужно:

    a) Открыть коммандную строку Git Bash и перейти в вашу папку-локальный репозиторий. Используйте команду cd.

   b) После того, как вы убедились, что находитесь в нужной папке, склонируйте репозиторий к себе командой ниже:
   ```
   git clone https://github.com/nustmisis/edu_python_nlp_2023
   ```
   c) В вашей папке должны появиться папка с файлами (edu_python_nlp_2023). Один из файлов называется ".git". Если такой файл находится в папке, это означает, что папка является git-репозиторием.
   Далее все свои действия вы будете производить непосредственно с той папкой, в которой лежит данный файл.

6. В Web-клиенте GitHub перейдите в раздел "Репозитории" и создайте там новый репозиторий. Он должен быть "Public".
7. Для того, чтобы отправить файлы из вашей локальной папки на удаленный репозиторий, перейдите в папку "edu_python_nlp_2023" и воспользуйтесь командами ниже.

   [ссылка] - это ссылка на ваш git-репозиторий. Пример: https://github.com/nustmisis/edu_python_nlp_2023
   
   Просто перейдите в ваш репозиторий и скопируйте её из адресной строки. Или после https://github.com/ добавьте ваш ник и через косую черту название вашего репозитория. 
  ```
git add .
git commit -m "first commit"
git remote add pythonrep [ссылка]
git push -u pythonrep main
   ```

Вуаля, вы восхитительны, файлы появились на удаленном клиенте. Можете обновить страницу репозитория и лицезреть вашу работу. 

Этого достаточно для того, чтобы начать работу с GitHub. Ниже вы найдете полезные (или не очень) подсказки по вашей дальнейшей работе с Git.

# Рутинная работа
Чаще всего вы будете добавлять/изменять/удалять файлы в вашей локальной папке на ПК. После этого вам нужно отправить изменения на удаленный клиент GitHub.

Ваша основная задача сводится к командам, предложенным ранее. Ниже перечислены основные шаги для внесения изменений в репозиторий.
1. Добавьте необходимые вам файлы в список для отправки на сервер. Это делается командой 
  ```
git add .
   ```
Точка в конце говорит о том, что добавятся все измененные файлы. Можно добавить конкретный файл:
  ```
git add filename
   ```
2. После этого нужно подтвердить, что эти файлы готовы для отправки. Используем команду *git commit*. В кавычках указывается короткий текст сообщения о сути внесенных изменений. 
```
git commit -m "your text"
   ```
3. Отправляем изменения на сервер командой
  ```
git push -u pythonrep main
   ```
main - название ветки, изменения в которой вы хотите закоммитить. Это основная ветка. Вы попадаете в неё по умолчанию. 
В данном случае *pythonrep* - название, которое мы ранее закрепили на нашим удаленным репозиторием. Можно добавить несколько репозиториев с разными названиями командой 
  ```
git remote add repository_name [ссылка]
   ```
и коммитить в разные репозитории, указывая их название. 

После этого новые изменения появляются в Web-версии GitHub. 

Подробнее про работу с Git Bash можно посмотреть [Здесь](https://www.youtube.com/watch?v=a1RzYqD8kBU&t=1005s&ab_channel=%D0%90%D0%B9%D1%82%D0%B8%D1%88%D0%BD%D0%B8%D0%BA%F0%9F%91%A9%E2%80%8D%F0%9F%92%BB)
или почитать [Здесь](https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud)
