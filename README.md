# Big-Data-Storage-and-Processing-Tools

# Lecturer
Timur Bosenko M. (bosenkotm@mgpu.ru)

Здесь Вы можете найти все материалы по дисциплине **`Инструменты для хранения и обработки больших данных`**. 

Курс представляет собой  введение в концепции анализа данных, роль аналитика данных и инструменты, которые используются для выполнения задач. Вы получите представление об экосистеме данных и основах анализа данных, таких как сбор данных или интеллектуальный анализ данных. Познакомитесь с современными инструментами аналитика данных, принципами работы инструментов бизнес-аналитики и BI-решений. Далее рассмотрим наиболее распространенное программное обеспечение и фреймворки (в основном это система `Hadoop`). В конце, когда Вы будете знать основные концепции и умеете настраивать и работать с распределенными средами и огромными наборами данных В конце каждого урока будут практические упражнения, которые мы начнем вместе и которые должны быть завершены к следующей встрече. 

## Программное обеспечение 

 - **`Google Colaboratory`** — бесплатная среда, чтобы писать код в jupyter notebook. [Google Colaboratory](  https://colab.research.google.com/).
 - **`Студия данных Google`** — cервис визуализации и анализа данных(En). [DataStudio](https://datastudio.google.com/navigation/reporting).
 - **`Yandex DataLens`** — cервис визуализации и анализа данных(Ru). [DataLens](https://datalens.yandex.ru/).
 - OC **`Ubuntu 20.04`** на базе кластера **`МГПУ`**. Номер РМ студента получить у ведущего лектора. Для работы потребуется клиент [anydesk](  https://anydesk.com/en/downloads/windows).
 - Инструкции и команды работы в [Docker containers](https://github.com/BosenkoTM/BigDataAnalitic_Practice/tree/main/docker22).

 `ВИРТУАЛЬНАЯ ГОСТЕВАЯ ОС`:
 
 - `D_System_22` [vm - VirtualBox](https://disk.yandex.ru/d/RTZvbDhtfXInMg), в его комплект входит:
    - `VirtualBox-6.1.30-148432-Win.exe` - ПО для разворачивания виртуальной ОС; 
    - `St_work_1.ova` - образ настроенной ОС `Ubuntu 18.04`;
    - `St_work_Hadoop.ova` - образ настроенной ОС `Ubuntu 18.04 + Hadoop`;
    - `login.txt`;
    - `ubuntu-18.04.6-desktop-amd64.iso` - исходный образ ОС.
 
 `Свободное программное обеспечение для бизнес-анализа`:
    - `Pentaho`[скачать](https://disk.yandex.ru/d/iVAdHZAPliBbkQ).

## Текущая успеваемость

 [АДЭУ-201]()

## Big-Data-Storage-and-Processing-Tools

- `lecture 01` Intro:
    -  [Intro](/lectures/lecture_01_1.pdf)
    -  [Big Data Storage](/lectures/lecture_01_2.pdf)

-  Practice: 
    -  01-1 [Визуализация данных из CSV-файла](https://cloud.yandex.ru/docs/datalens/tutorials/data-from-csv-visualization). [Индивидуальное задание](/practice/ex_01_1/01ex.md).
    -  01-2 [Product analytics](/practice/ex_01_2).
    
- `lecture 02`: 
    - [Инструменты интеграции и удаление файлов (ETL)](/lectures/lecture_02.pdf)
-  Practice: 
    - 02 [Работа в ETL-системе Talend](/practice/ex_02/pr_02_read_fileCSV_talend.pdf). Репозиторий программы [тут](https://disk.yandex.ru/d/jELYUXeI9HEEmg)
    
- `lecture 03`:
    - [Архитектура хранилищ данных: традиционная и облачная](/lectures/lecture_03.pdf)
-  Practice: 
    - 03 [Архитектура хранилищ данных: традиционная и облачная](/practice/ex_03/ex_3.pdf).  Pentaho DI требует установку Java 8. Попробуйте скачать архив и распаковать его. Вам нужно запустить spoon.sh для Linux/Mac и spoon.bat для Windows. Репозиторий программы [тут](https://disk.yandex.ru/d/jELYUXeI9HEEmg)

### Домашняя работа 1
Вам необходимо скачать и запустить Pentaho Data Integration Community Edition. Это бесплатный ETL инструмент, который работает на Windows, Linux и Mac. Вы можете скачать его [отсюда](https://sourceforge.net/projects/pentaho/). Pentaho DI требует установку Java 8. Попробуйте скачать архив и распаковать его. Вам нужно запустить spoon.sh для Linux/Mac и spoon.bat для Windows. У меня на Mac есть, например, иконка, `Data integration`.

Павел Новичков, ETL специалист, записал видео по установке Pentaho DI на примере Windows 10, с которым вы можете ознакомиться [здесь](https://www.youtube.com/watch?v=RL-EZCi51gc&feature=youtu.be&ab_channel=DataLearn)

### ETL Компоненты и начало работы с ETL на примере Pentaho Data Integration

ETL решения, требования и рекомендации, которые неплохо продумать перед началом создания data pipelines или data integration. 

**Видео лекция - теория** - [ETL Компоненты](https://youtu.be/-oCBttnefMQ). 

**Видео лекция - практика** - [Начало работы с Pentaho DI](https://youtu.be/-oCBttnefMQ?t=2087)

[Видео по основам Pentaho DI](https://youtu.be/K3X9wIC0jO8) и [ссылка на исходные файлы из видео](https://drive.google.com/file/d/1yw0E7Gqm4Rocui_pQYPdfmmnFtGfx3LY/view?usp=sharing)

### Домашняя работа 2
В качестве практики вам необходимо:
1. Скачать и запустить Pentaho DI, [отсюда](https://sourceforge.net/projects/pentaho/).
2. [Скачать примеры Pentaho jobs](https://github.com/Data-Learn/data-engineering/tree/master/DE-101%20Modules/Module04/DE%20-%20101%20Lab%204.4) для `Staging` и `Dimension Tables`.
3. Создайте еще одну трансформацию, в которой вы создадите `sales_fact` таблицу.

- `lecture 04`:
    - [Marketing Analytics - кейсы](https://github.com/pilosI/python_data_analysis#%D1%83%D1%87%D0%B5%D0%B1%D0%BD%D1%8B%D0%B5-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D1%8B-%D0%BF%D0%BE-%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%D1%83-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85-%D0%B2-jupyter-notebook)
-  Practice: 
    - 04-01 [Marketing Analytics](/marketing_analytics_students.ipynb).
    - 04-02 [Marketing Analytics vs MySQL](https://colab.research.google.com/drive/1ZFauMnc7JSRUGDEdor0EC6BAUe_YGVwt?usp=sharing).
    
- `lecture 05`:
    - [Business Intelligence-аналитика Data Prep & Alteryx Designer ](/lectures/lecture_05.pdf)
    
-  Practice:
 
   05 : Необходимо построить в `Tableau Prep Flow`, `Alteryx Workflow`потоки данных и сохранить результат в своем `git`. Вы можете использовать данные, подключившись к БД `Postgres` или БД `My SQL`, в которую мы загружали данные. Альтернативно, можете просто повторить существующие задания из Alteryx/Tableau tutorial, чтобы понять как работает инструмент.

    [Видеолекция по инструментам аналитики данных](https://www.tableau.com/support/releases/prep/2022.2.3#esdalt). 
    Репозиторий программы [тут](https://disk.yandex.ru/d/jELYUXeI9HEEmg)
    
    Дополнительные материалы для изучения:
    
    [Начало работы с Tableau prep](https://help.tableau.com/current/prep/en-us/prep_get_started.htm)
    
    [A-Practitioners-Guide-to-Tableau-prep-Builder](https://docs.yandex.ru/docs/view?tm=1665697499&tld=ru&lang=en&name=A-Practitioners-Guide-to-Tableau-prep-Builder.pdf&text=Tableau%20Prep&url=https%3A%2F%2Fresources.useready.com%2Fwp-content%2Fuploads%2F2019%2F08%2FA-Practitioners-Guide-to-Tableau-prep-Builder.pdf&lr=213&mime=pdf&l10n=ru&sign=6de6f2866532daf9d67052c949d1830f&keyno=0&nosw=1&serpParams=tm%3D1665697499%26tld%3Dru%26lang%3Den%26name%3DA-Practitioners-Guide-to-Tableau-prep-Builder.pdf%26text%3DTableau%2BPrep%26url%3Dhttps%253A%2F%2Fresources.useready.com%2Fwp-content%2Fuploads%2F2019%2F08%2FA-Practitioners-Guide-to-Tableau-prep-Builder.pdf%26lr%3D213%26mime%3Dpdf%26l10n%3Dru%26sign%3D6de6f2866532daf9d67052c949d1830f%26keyno%3D0%26nosw%3D1)
    
    [Начало работы с Alteryx Designer](https://help.alteryx.com/learn/learningguide.html)
    
- `lecture 06`:
    - [Инструменты аналитики Airflow + task on lecture_06](/lectures/lecture_06_airflow_day_1.pdf)
    
-  `Practice 06`: 
    -  [Live COVID-19 tracker with Airflow](https://towardsdatascience.com/your-live-covid-19-tracker-with-airflow-and-github-pages-658c3e048304).
    -  [Live COVID-19 tracker with Airflow GITHUB](https://github.com/hectoramirez/Covid19)
    
- `lecture 07`:
    - [Оркестр процессов обработки данных с помощью Apache Airflow](/lectures/lecture_07_airflow_day_2_orcestr.pdf)

### Дополнительные материалы для изучения

#### Apache Airflow
1. [Введение в Apache Airflow](https://khashtamov.com/ru/apache-airflow-introduction/) (Русский)
2. [Как мы оркестрируем процессы обработки данных с помощью Apache Airflow](https://habr.com/ru/company/lamoda/blog/518620/) (Русский)
3. [Apache Airflow: делаем ETL проще](https://habr.com/ru/post/512386/) (Русский)
4. [ETL процесс получения данных из электронной почты в Apache Airflow](https://habr.com/ru/post/495676/) (Русский)
5. [Getting started with Apache Airflow](https://towardsdatascience.com/getting-started-with-apache-airflow-df1aa77d7b1b) (English)
#### Apache NiFi
1. [Apache NiFi: что это такое и краткий обзор возможностей](https://habr.com/ru/company/rostelecom/blog/432166/) (Русский)
2. [Динамическое создание кластера Apache NiFi](https://habr.com/ru/post/331444/) (Русский)
3. [Apache NIFI — Краткий обзор возможностей на практике](https://habr.com/ru/post/465299/) (Русский)
4. [How Apache Nifi works — surf on your dataflow, don’t drown in it](https://medium.com/free-code-camp/nifi-surf-on-your-dataflow-4f3343c50aa2)
5. [Побег от скуки — процессы ETL](https://habr.com/ru/post/508620/) (Русский)
#### Data Build Tool (dbt) tool 
1. [Data Build Tool или что общего между Хранилищем Данных и Смузи](https://habr.com/ru/company/otus/blog/501380/) (Русский)
2. [DBT: A new way to transform data and build pipelines at The Telegraph](https://medium.com/the-telegraph-engineering/dbt-a-new-way-to-handle-data-transformation-at-the-telegraph-868ce3964eb4) (English)
3. [What, exactly, is dbt?](https://blog.getdbt.com/what--exactly--is-dbt-/) (English)
4. [Работа с dbt на базе Google BigQuery](https://habr.com/ru/post/542008/) (Русский)
5. [Сквозная Аналитика на Azure SQL + dbt + Github Actions + Metabase](https://habr.com/ru/post/538106/) (Русский)

#### Luigi
1. [Строим Data Pipeline на Python и Luigi](https://khashtamov.com/ru/data-pipeline-luigi-python/) (Русский)
2. [Обзор фреймворка Luigi для построения последовательностей выполнения задач](https://habr.com/ru/company/otus/blog/339904/) (Русский)
3. [Airbnb’s Airflow Versus Spotify’s Luigi](https://medium.com/better-programming/airbnbs-airflow-versus-spotify-s-luigi-bd4c7c2c0791) (English)
4. [Data pipelines, Luigi, Airflow: everything you need to know](https://towardsdatascience.com/data-pipelines-luigi-airflow-everything-you-need-to-know-18dc741449b7) (English)


## Теоретические вопросы

1.	Виды аналитики данных. Сравнительный анализ.
2.	Инструменты аналитики данных.
3.	Экосистема данных.
4.	Обзор экосистемы Data Analyst.Типы данных.
5.	Понимание различных типов форматов файлов.Источники данных.
6.	Языки для специалистов по данным.
7.	Обзор репозиториев данных.
8.	СУБД.NoSQL.
9.	Витрины данных, озера данных, ETL и конвейеры данных.
10.	Основы больших данных.
11.	Инструменты обработки больших данных.
12.	Инструменты сбора и обработки данных.
13.	Источники данных. Как собирать и импортировать данные.
14.	Что такое обработка данных. Инструменты для обработки данных. Очистка данных.
15.	Визуализация данных.
16.	Программное обеспечение для визуализации и информационной панели.
17.	Основные парадигмы теории Больших данных. Правило Мура. Правила Амдала. Виды распределенных систем в контексте больших данных.
18.	Распределенная файловая система Hadoop (`HDFS`).
19.	Менеджеры кластера: (`YARN`).
20.	Инструменты работы с большими данными `Hive` и  `HiveQL`.
21.	Инструменты работы с большими данными при пакетной обработке данных: Фреймворк `MapReduce`. 
22.	Инструменты работы с большими данными `Spark` и `PySpark`.
23.	Координатор: основные подходы при работе в `Zookeeper`.
24.	Инструменты работы с большими данными при потоковой передаче данных: `Apache Storm`, `Spark Streaming`, `Spark Structured Streaming`.
25.	Инструменты работы с большими данными на Графах: `Apache Giraph`, `Spark GraphX`.
26.	Контейнеры: основные подходы при работе  в `Docker`.

## ТЕСТ 1. 
[ССЫЛКА ДЛЯ ВХОДА](https://docs.google.com/forms/d/e/1FAIpQLSd0hfJDgqL1pNQE_np1S0V1_FVY7h_1Dvki7b_yimaj4Fnb8A/viewform?usp=sf_link)

## self-study

- `Семинар 1`. [Основные команды в Ubuntu](https://github.com/BosenkoTM/BigDataAnalitic_Practice/blob/main/common/docs/basic_shell_commands.md)
- [Альтернативное практическое изучение инструментов **Big Data**](https://github.com/BosenkoTM/BigDataAnalitic_Practice#practice)

## ТЕСТ 2. Apache Spark.

[ССЫЛКА ДЛЯ ВХОДА](https://docs.google.com/forms/d/e/1FAIpQLSdD_Hl-WwPK69VGKKf0tw1vF3AgMKYQRR3w9RofcIFKlJM4YA/viewform?usp=sf_link)

Вспомогательный материал:
 - [Источник 1](/books/test_books/Apache%2BZeppelin.pdf).

## ТЕСТ 3.
[ССЫЛКА ДЛЯ ВХОДА](https://docs.google.com/forms/d/e/1FAIpQLSdxADzRpGOzLrVBPHwUQMt6sWIPO63nLwYt0KolAWKq3-xREQ/viewform?usp=sf_link)

Вспомогательный материал:
 - [Источник 1](https://disk.yandex.ru/d/PFn19cqtOtn__g?w=1).

## Зачетное практическое задание по курсу  Big-Data-Storage-and-Processing-Tools

### `Вариант 1`

Использование `kaggle.com` Набора Данных **`Hubway`** Для Расчета Ключевых Показателей Эффективности Совместного Использования Велосипедов. [Условие задания](https://github.com/BosenkoTM/BigDataWork/blob/main/variant_1_exam_calculate/examp_1.pdf)

### `Вариант 2`

Использование данных **`NYC_Taxi`** для Расчета Ключевых Показателей Эффективности. [Условие задания](https://github.com/BosenkoTM/BigDataWork/blob/main/variant_2_exam_calculate/examp_2.pdf)

### `Вариант 3`

Настройка и работа в **`Hadoop`**, **`HDFS`** и **`Yarn`**. [Условие задания](https://github.com/BosenkoTM/BigDataWork/blob/main/variant_3_exam_calculate/examp_3.pdf)

### `Вариант 4`

Установка, настройка и работа в **`Hive`**. [Условие задания](https://github.com/BosenkoTM/BigDataWork/tree/main/variant_4_exam_calculate)


## Additional topics


- Linux and Python:
    - [Introduction to Linux Kernel](common/SysProg_Intro.pdf)
    - [Virtual File System](common/SysProg_VFS.pdf)
    - [Network Protocols](common/SysProg_NetworkProtocols.pdf)

## Summary table of literature sources
Разделы | 👨‍🏫 Курсы | 📚 Книги | 📊 Данные | 🙋‍♂️ Посты | ✊ Софт
--- | --- | --- | --- | --- | ---
Big Data | [Курсы по Big Data](books/courses_big_data.md) | [Книги по Big Data](books/software_big_data.md#книги-по-big-data) | + | [Источники, посвященные Big Data](books/social_data_science.md) | [Программы и библиотеки для работы с большими данными](/books/software_big_data.md#программы-и-библиотеки-для-bigdata)
