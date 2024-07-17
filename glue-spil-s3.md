В AWS Glue 2.0 окрім свіжих версій Apache Spark [завезли ще одну цікаву фічу](https://aws.amazon.com/blogs/big-data/introducing-amazon-s3-shuffle-in-aws-glue/). Раніше, під час виконання Apache Spark джоби, всі проміжні дані між стейджами зберігались на локальній файловій системі воркерів Glue кластера. При невідповідній конфігурації розмірів кластеру та великих масивів даних, які потрібно опрацювати, джоба зазвичай завершувалась неуспішно з помилкою `java.io.IOException: No space left on device`. Аби уникнути подібних ситуацій, можна було розширити розмір кластеру(збільшити місце на воркерах) або використати додатковий кластер для зберігання проміжних результатів.

У Glue 2.0 можна використати ще одну стратегію - зберігати проміжні дані на S3. Це дозволить уникнути будь-яких проблем з сховищем, там вимагає мінімум додаткової конфігурації.  