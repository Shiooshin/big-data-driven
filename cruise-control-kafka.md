У попередній компанії, коли ми розробляли near real-time систему з використанням Apache Kafka на власному залізі, управління та відлагодження кластеру було ручним, спираючись на JMX метрики. Зараз аби витрачати менше часу та зусиль існує інструмент під назвою Cruise Control. Про його основні фічі можна прочитати у [блозі компанії Cloudera](https://blog.cloudera.com/operating-apache-kafka-with-cruise-control/). Сruise Control дозволяє наприклад:
- легко додавати/видаляти брокери
- правильно відновлювати недоступні репліки
- має внутрішній механізм перевірки доступності брокерів і механізм відновлення брокерів при падінні.

Раніше, все вище згадане було описане десятками bash скриптів, які ми викликали, коли той чи інший алерт прилітав на пошту. Тепер це можна налаштувати комфортно і безболісно. 