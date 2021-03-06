---
title: Relational Databases
localeTitle: Реляционные базы данных
---
Поскольку база данных является способом хранения данных, реляционные базы данных являются моделью для хранения данных. Данные организованы в таблицы, также известные как отношения. Таблицы содержат запись для каждого экземпляра данных, известную как записи или кортежи. Уникальные идентификаторы идентифицируют каждую запись, чтобы описать ее через базу данных.

## таблицы

Как лист в excel, таблицы состоят из столбцов и строк. Каждая строка представляет собой экземпляр данных с атрибутами в столбце таблицы, которые известны как поля. Для каждой категории для нескольких объектов может быть несколько таблиц. Примером может служить таблица пользователей. Каждая строка будет пользователем, и каждое поле будет содержать сведения о пользователе, такие как адрес электронной почты, пароль и контактные данные для этого конкретного пользователя. На рисунке 1 вы можете увидеть схему примера.

| | пользователь | электронная почта | Телефон | | ------------- | ------------ | ------------------ | --- ----------------------------------- | | строка 1 | Джерри | j@j.uk.za | 771447444121 | | строка 2 | Салли | batgirl@gh.co.za | 771447444121 | | ряд 3 | Алекс | samwis@tty.fe | 771447444121 | | ряд 4 | Дуг | 4sure@dam.us | 745151515152 |

Рисунок 1 - Пример таблицы пользователя.

## документация

Запись - это единый объект данных. Как и в приведенном выше примере, это могут быть пользователь, учетная запись, устройство или все, что могут представлять данные. Записи нуждаются в уникальном идентификаторе, иногда называемом ключом. Этот ключ должен быть уникальным, поскольку он используется для описания отношений, которые запись имеет с другими записями в других таблицах. На рисунке 1 мы могли бы добавлять ключи к каждой строке, которая идентифицирует каждого пользователя с помощью ключа, а таблица теперь будет выглядеть как на рисунке 2.

| КЛЮЧ | пользователь | электронная почта | Телефон | | ----------- | ------------ | ------------------ | ----- --------------------------------- | | u1 | Джерри | j@j.uk.za | 771447444121 | | u2 | Салли | batgirl@gh.co.za | 771447444121 | | u3 | Алекс | samwis@tty.fe | 771447444121 | | u4 | Дуг | 4sure@dam.us | 745151515152 |

Рисунок 2 - Пример пользовательской базы данных с полем KEY.

## поля

Поля описывают запись. Это может содержать любую информацию о сущности, которая символизирует запись. На рисунке 3 вы можете увидеть таблицу, в которой показаны домашние животные. Столбцы (поля) описывают каждое домашнее животное (запись) с p\_name, p\_age, p\_type и p\_owner. P является сокращением для домашнего животного, и последний столбец будет объяснен в следующем разделе о взаимоотношениях.

| КЛЮЧ | p\_name | p\_age | p\_owner | | ----------- | ------------ | ------------------ | ----- ---------- | | p1 | Сьюзи | j@j.uk.za | u1 | | p2 | Маленький Dip | batgirl@gh.co.za | u1 | | p3 | Amillë | samwis@tty.fe | u2 | | p4 | Дуг | 4sure@dam.us | u3 |

Рисунок 3 - Пример стола для домашних животных.

## Отношения

Реляционные базы данных позволяют описывать отношения, которые имеют отношения друг с другом. Иногда это самая сложная тема для реляционных баз данных. Если мы возьмем наши таблицы примеров, мы сможем увидеть взаимосвязь нашей таблицы пользователей с таблицей домашних животных. Если вы читаете поле p\_owner, вы можете видеть, что оно также может быть таким же, как на рисунке 4. Это объясняет отношение, которое каждое домашнее животное имеет с пользователем. Отношения могут иметь разные типы.

| КЛЮЧ | p\_name | p\_age | p\_owner | | ----------- | ------------ | ------------------ | ----- ---------- | | p1 | Сьюзи | j@j.uk.za | Джерри | | p2 | Маленький Dip | batgirl@gh.co.za | Джерри | | p3 | Amillë | samwis@tty.fe | Салли | | p4 | Дуг | 4sure@dam.us | Дуг |

Рисунок 4 - Пример таблицы Pet с подключенным полем владельца.

Отношение «один ко многим» - это одна запись, связанная со многими другими записями, примером которой является пользователь Джерри с двумя домашними животными. Это также может быть отношение «многие ко многим», где таблицы могут быть книгами и авторами, поскольку авторы могли бы написать много книг. Наконец, наиболее распространенный тип отношений - это один к одному, запись, которая может быть связана только с одной и только с одной, другой записью.

## Вывод

Это всего лишь краткое введение в реляционные базы данных. Ниже приведены ссылки на ресурсы, которые могут помочь вам продолжить изучение предмета.

#### Дополнительная информация:

*   Реляционные базы данных по [википедии](https://en.wikipedia.org/wiki/Relational_database)
*   Один-ко-многим в [Википедии](https://en.wikipedia.org/wiki/One-to-many_(data_model) )
*   Многие-ко-многим в [Википедии](https://en.wikipedia.org/wiki/Many-to-many_(data_model) )
*   Один-к-одному в [Википедии](https://en.wikipedia.org/wiki/One-to-one_(data_model) )
*   Модель отношения к [википедии](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model)