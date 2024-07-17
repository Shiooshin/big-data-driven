Повз мене пройшла новина, що AWS Glue тепер має Schema Registry. Перше, що приходило в голову - це писати свій менеджер схем і зберігати схеми на файловому сховищі з увімкненим версіонуванням. Якщо було більше часу і можливостей - я розглядав варіант з [Confluent Schema Registry](https://docs.confluent.io/platform/current/schema-registry/index.html). Не знаю як зараз, але раніше в Confluent Schema Registry були жахливі проблеми з HA і декілька інстансів Registry не могли поділити топік з схемами. 

Тепер це все можна без проблем організувати через AWS Glue. Також Glue надає API для інтеграції: до Registry можна доступитись з Glue Catalog, Kinesis, MSK та Lambda. І віднедавна, AWS Glue окрім Avro схем, [підтримує plain JSON схеми](https://aws.amazon.com/about-aws/whats-new/2021/06/aws-glue-schema-registry-now-supports-json-schema/), що дуже зручно, коли завдання якомога простіше сконфігурувати схему даних.

AWS не бере грошей за використання Schema Registry, проте будьте уважні з **лімітами** сервісу щодо схем:
- ***You can have up to 10 registries per AWS account per AWS Region.***
- ***There is a size limit of 170KB for schema payloads.***
- ***you can theoretically have up to 1000 schemas per account per region, if each schema has only one version.***