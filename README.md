***Результаты выполнения команд***
=


**Подключение к контейнеру**
-
docker exec -it 03a73d08cb46 bash


**Копирование предварительно объединенного файла книги в hdfs**
-
1) docker cp voyna-i-mir-tom-1.txt 03a73d08cb46 **(вне контейнера)**
2) hadoop fs -put voyna-i-mir-tom-1.txt /user/lapis


**Проверка наличия файла после перемещения**
-
![](https://github.com/lapisgame/4.4_hadoop_hive/blob/master/res_img/1%20Снимок%20экрана%20от%202023-09-02%2000-09-05.png?raw=true)


**Установка параметров доступа 755 (Владелец - полный доступ, остальные - чтение запись)**
-
![](https://github.com/lapisgame/4.4_hadoop_hive/blob/master/res_img/2%20Снимок%20экрана%20от%202023-09-02%2000-11-11.png?raw=true)


**Проверка занимаемого дискового пространства с фактором репликации 3**
-
![](https://github.com/lapisgame/4.4_hadoop_hive/blob/master/res_img/3%20Снимок%20экрана%20от%202023-09-02%2000-12-26.png?raw=true)


**Изменения фактора репликации на 2 и проверка места**
-
![](https://github.com/lapisgame/4.4_hadoop_hive/blob/master/res_img/4%20Снимок%20экрана%20от%202023-09-02%2000-14-45.png?raw=true)


**Вывод количества строк в файле на экран**
-
![](https://github.com/lapisgame/4.4_hadoop_hive/blob/master/res_img/5%20Снимок%20экрана%20от%202023-09-02%2000-16-07.png?raw=true)