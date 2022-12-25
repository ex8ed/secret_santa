# <b>ТАЙНЫЙ САНТА. Киберпомощник</b>
***
## Краткое введение

Это приложение появилось в порыве облегчить распределение ~~варваров~~ детей и
избавиться от предновогоднего геморроя после создания анкеты. 

Для того чтобы получить готовые сообщения с тем, что было в анкете, достаточно
импортировать файл с таблицей и получить в консоли результат, чтобы оперативно отправить.

Я решил сделать эту программу с расчетом на то, что это происходит каждый год и инструмент,
позволяющий сделать процесс легким и автоматическим не помешает.

<mark>***ДЛЯ РАБОТЫ ПРОГРАММЫ ВАМ ПОНАДОБИТСЯ УСТАНОВИТЬ ИНТЕРПРЕТАТОР PYTHON НЕ НИЖЕ 3.8!!!*** </mark>

<mark>***ВСЕ НЕОБХОДИМЫЕ БИБЛИОТЕКИ УКАЗАНЫ В  requirements.txt*** </mark>

>Внимание! Автор данного микро-руководства предполагает, что вы уже создали 
> гугл форму и имеете данные из таблицы. В противном случае вам следует 
> сдвинуться на шаг назад, если вы решили выбрать Google Forms. Если нет: ваш
> способ - херня, выберите Google Forms.
 
>Очень важно добавить, что сработает это для гугл-формы образца года 2021 ~~(а то я что, просто так это писать сел?)~~.
Если вы горите желанием полностью автоматизировать процесс, то возможны два исхода:
>>- вы просто поправляете адреса ячеек в скрипте ***message_generator*** 
(для комплюктерных гениев)

## Описание файлов
В ***config.py*** лежит шаблон отправляемого сообщения. Редактировать его нужно там.


В файле ***main.py*** производится деление детей на пары. Все просто - вам необходимо внести 
все правки ***config.py*** и запустить скрипт - ~~петухон~~ самый мощный
и легко читаемый промышленный язык программирования все сделает за вас.

> Если вас по каким-то причинам не устраивает результат программы, то вызовите ее еще раз -
> каждый раз результат окажется рандомным.


> Вы не обязаны пользоваться текущим шаблоном, ~~написанным на коленке под пиво~~,
> который показался автору наиболее удобным.
> Оно содержится прямо в начале файла - вам достаточно изменить его содержание в тройных кавычках.

Перед тем, как начать работу, скачайте гугл-таблицу и передайте в конструктор полный путь. По умолчанию используется
<mark><samp>./data.xlsx</samp></mark> Также необходимо условиться о том, как именно вы назовете столбцы. Это легко
меняется, но поправить будет необходимо. Поверьте, вы интуитивно поймете, где это надо сделать. 
В противном случае просто ничего не запустится.

> Я не стал делать работу с .csv файлами просто для конечного удобства пользователя. Этим необязательно будет заниматься
> человек, готовый ~~мудохаться~~ разбираться с файлами и расширениями.

Все данные выводятся в файл <mark><samp>messages.txt</samp></mark> - как только манипуляции завершены, вы можете смело
скопировать из него получившиеся сообщения 
и отправлять по готовому списку. 

Счастливого вам нового года!

(с) Киберпомощник тайного санты.
