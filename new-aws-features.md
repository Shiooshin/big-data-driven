Сьогодні в двох словах про новинки від AWS:
- Для популярного ORM фреймворку для Python, SQLAlchemy, [з'явився redshift діалект](https://aws.amazon.com/blogs/big-data/use-the-amazon-redshift-sqlalchemy-dialect-to-interact-with-amazon-redshift/). Тепер можна підключитись через SQLAlchemy до Redshift використовуючи IAM та SSO. Також доступні специфічні для Redshift команди як от SUPER, GEOMETRY, TIMESTAMPTZ, and TIMETZ.
- Тепер [індексування партицій доступне для Athena](https://aws.amazon.com/blogs/big-data/use-the-amazon-redshift-sqlalchemy-dialect-to-interact-with-amazon-redshift/). При виконанні Athena запиту, інформацію щодо розташування партицій можна отримати значно швидше з Glue Catalog. Для цього не потрібно перестворювати таблицю в Glue Catalog, а лише створити новий індекс для існуючої таблиці. 