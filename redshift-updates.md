На відміну від версійних релізів, AWS викатує новинки як тільки вони готові. Тож цього разу маємо нові фічі для:
- **Amazon Redshift**
    - Тут насправді купа нового і цікавого. [Анонсовано підтримку LakeFormation для Redshift таблиць](https://aws.amazon.com/about-aws/whats-new/2023/04/amazon-redshift-access-control-data-sharing-lake-formation/). Він поширюється як на нативні таблиці, так і на таблиці що зберігаються в S3 і доступні для запитів через Redshift Spectrum.
    - [Анонсовано MERGE SQL команду](https://aws.amazon.com/about-aws/whats-new/2023/04/amazon-redshift-availability-merge-sql-command/) для збільшення атомарності DML стейтментів.
    - [В беті знаходиться Dynamic Data Masking](https://aws.amazon.com/about-aws/whats-new/2023/04/amazon-redshift-availability-dynamic-data-masking/). Такий функціонал нещодавно викотили в BigQuery. DDM дозволяє під час запиту замаскувати певні колонки, які можуть бути sensitive. 
    - [Неймовірний буст запитів до рядкових літералів](https://aws.amazon.com/about-aws/whats-new/2023/04/amazon-redshift-string-query-performance-up-to-63x/). Обіцяють, що особливо добре працює з low cardinality літералами.
- **AWS Glue**
    - [Тепер вміє створювати автоматично добавляти партиціонування до нових таблиць](https://aws.amazon.com/about-aws/whats-new/2023/04/aws-glue-crawlers-creating-partition-indexes/), які підхоплює Glue Crawler.

