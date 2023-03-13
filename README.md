# ZakupkiOrganizaciiCemMatcher
Check companies in public registry - https://zakupki.gov.ru/ and http://fas.gov.ru/

**Парсер** (ветка master)

Используется Java 15.

На данный момент реализована возможность проверки организаций на сайтах - https://zakupki.gov.ru/ и http://fas.gov.ru/ 
на регистрацию организаций в реестрах на 223-ФЗ и 44-ФЗ:
1. "Реестр заказчиков"; 
2. "Реестре организаций";
3. "Реестре сведений об объеме выручки";
4. "Реестре субъектов естесственных монополий"

Данные берутся напрямую с сайтов, так как данные на ftp сервере не всегда соответствуют действительности.

**Запуск** 

1. Напрямую из среды разработки с настройкой проекта Maven и вводом excel файла (.xls) с данными - ОГРН, 
полное (или сокращенное) наименование организации (1 столбец и 2 столбец).

2. Запуск jar файла, так как формируется fat jar, с указанием файла excel (.xls) - с данными - ОГРН,
полное (или сокращенное) наименование организации (1 столбец и 2 столбец).

**Пример .xsl файла**

https://github.com/github/maupa13/ZakupkiOrganizaciiCemMatcher/blob/excel-example.png