На днях офіційно вийшов [новий реліз Apache kafka 3.0.0](https://www.confluent.io/blog/apache-kafka-3-0-major-improvements-and-new-features/). Стаття містить опис найбільших змін. З основного:
- exactly once за замовчуванням (дивно, але тепер це звучить як stronger consistency а не як exactly once delivery)
- поступова відмова від Java 8 та Scala 2.12 (покищо deprecated, з версії 4.0 не буде підтримуватись взагалі)
- підтримка серіалізації/десеріалізації List<T> колекції 
- також зміни у супутніх сервісах: Kafka Streams, Kafka Connect та MirrorMaker