GCP все ближче наближається до AWS по різноманітності сервісів пов'язаних з обробкою даних, чи точніше сказати Spark. Рвніше GCP в своєму арсеналі мав тільки Hadoop-as-a-Service і Apache Beam. Я нещодавно писав, що в ранньому доступі вже з'явився аналог AWS Glue, який GCP активно розвиває: [нова стаття](https://cloud.google.com/blog/products/data-analytics/making-serverless-spark-even-more-powerful) у GCP блозі про:
- перехід Serverless Spark від стадії раннього доступу до публічного доступу
- більшу кількість інтеграцій для Seeverless Spark з сервісами BigQuery, Dataproc, Dataplex та Vertex AI
- і неочікуваний анонс Dataproc на Kubernetes(GKE)

Такими темпами віддзеркалення сервісів обробки великих даних ми в найближчому майбутньому прийдемо до cloud-agnostic ETL пайплайнів на Spark + Terraform. І окремиою архітектурою ETL для Azure Cloud.