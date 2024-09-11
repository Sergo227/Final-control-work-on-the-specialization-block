# Final-control-work-on-the-specialization-block

# `Итоговая контрольная работа`

## `Информация о проекте`
Необходимо организовать систему учета для питомника, в котором живут домашние и вьючные животные.

## `Задание:`

### 1. Используя команду cat, в терминале операционной системы Linux создать два файла Домашние животные (заполнив файл собаками, кошками, хомяками) и Вьючные животными (заполнив файл лошадьми, верблюдами и ослами), а затем объединить их. Просмотреть содержимое созданного файла. Переименовать файл, дав ему новое имя (Друзья человека).

cat > 'Домашние животные'

В открывшемся файле указываем
Собаки
Кошки
Хомяки

cat > 'Вьючные животные'

В открывшемся файле указываем
Лошади
Верблюды
Ослы

cat 'Домашние животные' 'Вьючные животные' > Животные

ls

mv Животные 'Друзья человека'

ls

### 2. Создать директорию, переместить файл туда.

mkdir newdir

mv 'Друзья человека' newdir/

ls

##### root@mfedko:/home/mfedko/Desktop# cat > 'Домашние животные'
##### Собаки
##### Кошки
##### Хомяки
##### ^C
##### root@mfedko:/home/mfedko/Desktop# cat > 'Вьючные животные'
##### Лошади
##### Верблюды
##### Ослы
##### ^C
##### root@mfedko:/home/mfedko/Desktop# cat Домашние\ животные Вьючные\ животные > 'Животные'
##### root@mfedko:/home/mfedko/Desktop# cat Животные
##### Собаки
##### Кошки
##### Хомяки
##### Лошади
##### Верблюды
##### Ослы
##### root@mfedko:/home/mfedko/Desktop# mv Животные 'Друзья человека'
##### root@mfedko:/home/mfedko/Desktop# mkdir newdir
##### root@mfedko:/home/mfedko/Desktop# mv Друзья\ человека newdir/
##### root@mfedko:/home/mfedko/Desktop# tree
##### .
##### ├── commands
##### ├── hw_script
##### ├── newdir
##### │   └── Друзья человека
##### ├── wordpress
##### │   └── docker-compose.yml
##### └── nginx-conf
#####     ├── nginx.conf
#####     └── options-ssl-nginx.conf
##### ├── Вьючные животные
##### └── Домашние животные



### 3. Подключить дополнительный репозиторий MySQL. Установить любой пакет из этого репозитория.

1. Установка репозитория:
    wget -c https://dev.mysql.com/get/mysql-apt-config_0.8.17-1_all.deb
    sudo dpkg -i mysql-apt-config_0.8.17-1_all.deb
    sudo apt-get update
    
2. Установка пакета из репозитория:
    sudo apt-get install mysql-server
    
3. Проверяем результат установки:

systemctl status mysql

### 4. Установить и удалить deb-пакет с помощью dpkg.

1. Установка пакета:
    
    wget -c <URL деб-пакета>
    sudo dpkg -i <пакет.deb>
    
2. Удаление пакета:
    
    sudo dpkg -r <имя_пакета>
    
Скачиваем пакет для установки:

wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb

Устанавливаем пакет mysql-connector-j_8.0.32-1ubuntu22.04_all.deb:

sudo dpkg - i mysql-connector-j_8.0.32-1ubuntu22.04_all.deb

Удаляем пакет и его сопутствующие пакеты:

sudo dpkg -r mysql-connector-j

sudo apt-get autoremove

##### wget https://dev.mysql.com/get/mysql-apt-config_0.8.24-1_all.deb
##### cd Downloads/
##### sudo dpkg -i mysql-apt-config_0.8.24-1_all.deb
##### sudo apt-get update

##### sudo apt-get install mysql-server
##### systemctl status mysql
##### wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
##### sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
##### sudo dpkg -r mysql-connector-j
##### sudo apt-get autoremove


### 5. Выложить историю команд в терминале ubuntu.

Для получения истории введенных команд в терминале ubuntu используем:

history

49  cat > 'Домашние животные'
50  cat > 'Вьючные животные'
51  cat Домашние\ животные Вьючные\ животные > 'Животные'
52  cat Животные
53  mv Животные 'Друзья человека'
54  mkdir newdir
55  mv Друзья\ человека newdir/
56  tree
57  wget https://dev.mysql.com/get/mysql-apt-config_0.8.24-1_all.deb > commands
58  cat > commands
59  rm commands
60  cat > commands
61  history
62  wget https://dev.mysql.com/get/mysql-apt-config_0.8.24-1_all.deb
63  cd Downloads/
64  cd ..
65  cd ..
66  cd ..
67  cd ..
68  cd ..
69  cd Downloads/
70  ls
71  sudo dpkg -i mysql-apt-config_0.8.24-1_all.deb
72  sudo apt-get update
73  sudo dpkg -i mysql-apt-config_0.8.24-1_all.deb
74  sudo dpkg --configure -a
75  sudo dpkg -i mysql-apt-config_0.8.24-1_all.deb
76  sudo apt-get update
77  sudo apt-get install mysql-server
78  systemctl status mysql
79  wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
80  sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
81  sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
82  sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
83  sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
84  sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
85  sudo dpkg -i ~/Загрузки/mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
86  sudo dpkg -r mysql-connector-j
87  sudo apt-get autoremove
88  sudo dpkg -i mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
89  sudo dpkg -r mysql-connector-j
90  sudo dpkg -i mysql-connector-j_8.0.32-1ubuntu22.04_all.deb
91  sudo dpkg -r mysql-connector-j
92  sudo apt-get autoremove
93  sudo apt-get autoremove
94  history

### 6. Нарисовать диаграмму, в которой есть класс родительский класс, домашние животные и вьючные животные, в составы которых в случае домашних животных войдут классы: собаки, кошки, хомяки, а в класс вьючные животные войдут: лошади, верблюды и ослы).

[https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1#G1-gEMiji0-sIQ_MWsWpHr--5FpARTW7Vr]

### 7. В подключенном MySQL репозитории создать базу данных "Друзья человека"

### 8. Создать таблицы с иерархией из диаграммы в БД.

### 9. Заполнить низкоуровневые таблицы именами (животных), командами, которые они выполняют, и датами рождения.

### 10. Удалив из таблицы верблюдов, т.к. верблюдов решили перевезти в другой питомник на зимовку, объединить таблицы лошади и ослы в одну таблицу.

### 11. Создать новую таблицу “молодые животные”, в которую попадут все животные старше 1 года, но младше 3 лет и в отдельном столбце с точностью до месяца подсчитать возраст животных в новой таблице.

### 12. Объединить все таблицы в одну, при этом сохраняя поля, указывающие на прошлую принадлежность к старым таблицам.
#### Решение с 8-12 задания представлены ниже:
USE peoplefriends;

CREATE TABLE cat (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE
);

CREATE TABLE dog (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE
);

CREATE TABLE hamster (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE
);

CREATE TABLE horse (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE
);

CREATE TABLE camel (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE
);

CREATE TABLE donkey (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE
);

INSERT INTO cat (animal_name,commands, date_of_birth) VALUES 
	('barsik', 'meow', '2021-01-01'),
	('kosh', 'meow, stand', '2019-12-10'),
    ('frank', 'meow, wlow', '2020-02-02'),
    ('dir', 'meow', '2022-03-03'),
    ('krop', 'meow', '2018-05-05');
   
INSERT INTO dog (animal_name,commands, date_of_birth) VALUES 
	('wolf', 'flufy', '2021-01-01'),
	('ralf', 'site', '2019-12-10'),
    ('qwerty', 'left hand', '2020-02-02'),
    ('asdfg', 'right hand', '2022-03-03'),
    ('red', 'meow', '2018-05-05');
    
INSERT INTO hamster (animal_name,commands, date_of_birth) VALUES 
	('crack', 'eat', '2021-01-01'),
	('jisus', 'eat', '2019-12-10'),
    ('qwerty', 'left hand', '2020-02-02'),
    ('asdfg', 'right hand', '2022-03-03'),
    ('black', 'meow', '2018-05-05');
    
INSERT INTO horse (animal_name,commands, date_of_birth) VALUES 
	('igogo', 'eat', '2021-01-01'),
	('igaga', 'eat', '2019-12-10'),
    ('ijoho', 'left hand', '2020-02-02'),
    ('jijij', 'right hand', '2022-03-03'),
    ('aoaoaa', 'meow', '2018-05-05');
    
INSERT INTO camel (animal_name,commands, date_of_birth) VALUES 
	('qwea', 'eat', '2021-01-01'),
	('dsaf', 'eat', '2019-12-10'),
    ('gfdsdf', 'left hand', '2020-02-02'),
    ('grwtw', 'right hand', '2022-03-03'),
    ('werqr', 'meow', '2018-05-05');
    
INSERT INTO donkey (animal_name,commands, date_of_birth) VALUES 
	('stup', 'eat', '2021-01-01'),
	('tupi', 'eat', '2019-12-10'),
    ('upid', 'left hand', '2020-02-02'),
    ('task', 'right hand', '2022-03-03'),
    ('done', 'meow', '2018-05-05');
    
TRUNCATE camel;

INSERT INTO horse (animal_name, commands, date_of_birth)
SELECT animal_name, commands, date_of_birth
FROM donkey;

DROP TABLE donkey;

RENAME TABLE horse TO horse_donkey;

CREATE TABLE young_animal (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE,
    age TEXT
);


DELIMITER $$
CREATE FUNCTION age_animal (date_b DATE)
RETURNS TEXT
DETERMINISTIC
BEGIN
    DECLARE res TEXT DEFAULT '';
	SET res = CONCAT(
            TIMESTAMPDIFF(YEAR, date_b, CURDATE()),
            ' years ',
            TIMESTAMPDIFF(MONTH, date_b, CURDATE()) % 12,
            ' month'
        );
	RETURN res;
END $$
DELIMITER ;

INSERT INTO young_animal (animal_name, commands, date_of_birth, age)
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth)
FROM cat
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3
UNION ALL
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth)
FROM dog
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3
UNION ALL
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth)
FROM hamster
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3
UNION ALL
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth)
FROM horse_donkey
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3;

SET SQL_SAFE_UPDATES = 0;

DELETE FROM cat 
WHERE TIMESTAMPDIFF(YEAR, cat.date_of_birth, CURDATE()) IN (1, 2, 3);

DELETE FROM dog 
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3;

DELETE FROM hamster 
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3;

DELETE FROM horse_donkey 
WHERE TIMESTAMPDIFF(YEAR, date_of_birth, CURDATE()) BETWEEN 1 AND 3;

CREATE TABLE animals (
	id INT PRIMARY KEY AUTO_INCREMENT,
	animal_name CHAR(30),
    commands TEXT,
    date_of_birth DATE,
    age TEXT,
    animal_type ENUM('cat','dog','hamster', 'horse_donkey', 'young_animals') NOT NULL
);

INSERT INTO animals (animal_name, commands, date_of_birth, age, animal_type)
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth), 'cat'
FROM cat;

INSERT INTO animals (animal_name, commands, date_of_birth, age, animal_type)
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth), 'dog'
FROM dog;

INSERT INTO animals (animal_name, commands, date_of_birth, age, animal_type)
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth), 'hamster'
FROM hamster;

INSERT INTO animals (animal_name, commands, date_of_birth, age, animal_type)
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth), 'horse_donkey'
FROM horse_donkey;

INSERT INTO animals (animal_name, commands, date_of_birth, age, animal_type)
SELECT animal_name, commands, date_of_birth, age_animal(date_of_birth), 'young_animals'
FROM young_animal;

### 13. [Создать класс](Animals) с Инкапсуляцией методов и наследованием по диаграмме.

### 14. Написать программу, имитирующую работу реестра домашних животных.
В программе должен быть реализован следующий функционал:

#### 14.1. Завести новое животное
#### 14.2. Определять животное в правильный класс
#### 14.3. Увидеть список команд, которое выполняет животное
#### 14.4. Обучить животное новым командам
#### 14.5. Реализовать навигацию по меню

- Реализовано взаимодействие с БД. Пункты: 
  - 14.1
  - 14.2
  - 14.3
  - 14.4 

- Интерфейс в разработке.

- Для работы с БД, необходимо внести данные подключения к БД в [конфигурационный файл](db/ConnectData.java)

### 15. Создайте класс Счетчик, у которого есть метод add(), увеличивающий значение внутренней int переменной на 1 при нажатии "Завести новое животное". Сделайте так, чтобы с объектом такого типа можно было работать в блоке try-with-resources. Нужно бросить исключение, если работа с объектом типа счетчик была не в ресурсном try и/или ресурс остался открыт. Значение считать в ресурсе try, если при заведении животного заполнены все поля.

public class Counter implements AutoCloseable {
    private int count = 0;
    private boolean isClosed = false;
    private boolean isUsedInTryWithResources = false;

    public void add() {
        if (isClosed) {
            throw new IllegalStateException("Cannot use Counter after it has been closed.");
        }
        count++;
    }

    @Override
    public void close() {
        if (!isUsedInTryWithResources) {
            throw new IllegalStateException("Counter was not used in a try-with-resources block.");
        }
        isClosed = true;
        System.out.println("Counter closed.");
    }

    // This method is for internal use to mark the counter as used in try-with-resources
    void markUsedInTryWithResources() {
        isUsedInTryWithResources = true;
    }

    public int getCount() {
        return count;
    }

    // Simulate animal creation with required fields check
    public static void createNewAnimal(Counter counter, String name, String dateOfBirth, String... commands) throws IllegalArgumentException {
        if (name == null || name.isEmpty() || dateOfBirth == null || dateOfBirth.isEmpty() || commands == null || commands.length == 0) {
            throw new IllegalArgumentException("All fields must be filled to create a new animal.");
        }
        counter.add();
        System.out.println("New animal created: " + name);
    }

    public static void main(String[] args) {
        try (Counter counter = new Counter()) {
            counter.markUsedInTryWithResources();
            createNewAnimal(counter, "Dog", "2021-01-01", "Sit", "Stay");
            createNewAnimal(counter, "Cat", "2022-02-02", "Jump");
            System.out.println("Count: " + counter.getCount());
        } catch (IllegalArgumentException | IllegalStateException e) {
            System.err.println(e.getMessage());
        }
    }
}

В этом примере:

1. Класс Counter реализует интерфейс AutoCloseable, чтобы его можно было использовать в блоке try-with-resources.
2. Метод add() увеличивает внутреннюю переменную count на 1.
3. Метод close() проверяет, был ли счетчик использован в блоке try-with-resources и закрывает его.
4. Метод markUsedInTryWithResources() отмечает счетчик как используемый в try-with-resources.
5. Метод createNewAnimal() симулирует создание нового животного и увеличивает счетчик, если введены все необходимые данные.
