# Связи между элементами многоуровневого картежа
## Задача:
Дан массив пользователей. Необходимо реализовать функцию, которая принимает на вход три аргумента:</br>
- информация о связях,кортеж (tuple) кортежей,</br>
- первое имя (str),
- второе имя (str).</br>

Функция должна возвращать **True**, 
если связь между любыми заданными пользователями существует,
например, если у двух пользователей есть общие друзья 
или у их друзей есть общие друзья и т.д., иначе **False**
#### Данные:
<image src="static/images/Данные.JPG" alt="Данные для решения задачи">


## Решение:
1) Создаем пустое множество *frends = set()* и 
в него добавляется первое искомое имя *frends.add(first)*
2) Создаем цикл *while*. Цикл останавливается, 
когда во множестве *frends* больше не добавляются новые имена. 
3) В цикле *while* создаем новый цикл *for* в котором итерируем
значения кортежа *net*. Во вложенных картежах достаем каждый элемент
и проверяем на коллизии с множеством *frends*. Если коллизии есть, то 
добавляем текущий вложенный кортеж в созданное множество *frends*
 



