# Домашнее задание к занятию 10 «Jenkins»

## Основная часть

1. Сделать Freestyle Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.  
<img src="./job1_1.png"/>
<img src="./job1_2.png"/>
2. Сделать Declarative Pipeline Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.
<img src="./job2_1.png"/>
<img src="./job2_2.png"/>
<img src="./job2_3.png"/>

3. Перенести Declarative Pipeline в репозиторий в файл [Jenkinsfile](./Jenkinsfile).
<img src="./job3_1.png"/>
<img src="./job3_2.png"/>
4. Создать Multibranch Pipeline на запуск `Jenkinsfile` из репозитория.
<img src="./job4_1.png"/>
<img src="./job4_2.png"/>
<img src="./job4_3.png"/>
5. Создать Scripted Pipeline, наполнить его скриптом из [pipeline](./pipeline).
6. Внести необходимые изменения, чтобы Pipeline запускал `ansible-playbook` без флагов `--check --diff`, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и запускает прогон с флагами `--check --diff`.
<img src="./job5_1.png"/>
<img src="./job5_2.png"/>
<img src="./job5_3.png"/>
8. Отправить ссылку на репозиторий с ролью и Declarative Pipeline и Scripted Pipeline.  
[Scripted_Pipeline](ScriptedJenkinsfilene)



