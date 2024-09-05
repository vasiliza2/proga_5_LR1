# Лабораторная работа №1. Реализация удаленного импорта собственного пакета

1.Создали файл myremotemodule.py, который будет импортироваться, разместили его в каталоге, который далее будет "корнем сервера".
Разместиkb в нём необходимый код
![Image1](https://github.com/vasiliza2/proga_5_LR1/blob/76668a338e99b20a10b6f682f16aaa75aef06c07/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-09-05%20150228.png)

2. Создали файл Python с содержимым функций url_hook и классов URLLoader, URLFinder из текста конспекта лекции со всеми необходимыми библиотеками
![image2](https://github.com/vasiliza2/proga_5_LR1/blob/ce90d94bb8679aaa341ed7dbc9fa1248b84b0e4e/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-09-05%20151611.png)
![image3](https://github.com/vasiliza2/proga_5_LR1/blob/ce90d94bb8679aaa341ed7dbc9fa1248b84b0e4e/image.png)

3. Далее, чтобы продемонстрировать работу импорта из удаленного каталога, мы запустили сервер http так, чтобы наш желаемый для импорта модуль "лежал" на сервере.  Открыли каталог rootserver с файлом myremotemodule.py и запустили там сервер:
python3 -m http.server
![image4](https://github.com/vasiliza2/proga_5_LR1/blob/94a94fc9f690de4362692987a013dffa2ce909b8/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-09-05%20143821.png)

4. После этого мы запустили файл, в котором содержится код.
python3 -i activation_script.py
 
Выполнили код:
sys.path.append("http://localhost:8000")

![image5](https://github.com/vasiliza2/proga_5_LR1/blob/94a94fc9f690de4362692987a013dffa2ce909b8/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-09-05%20143837.png)

![image6](https://github.com/vasiliza2/proga_5_LR1/blob/e2f051fa3a0ab0ffc031517b125c381ae3c6d1d7/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-09-05%20143737.png)
