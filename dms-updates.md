Дрібні радощі від AWS. Тепер DMS(Database Migration Service) має дві нові фічі:
- під час CDC режиму, коли дані з джерела переливаються з джерела на S3, DMS сам [валідує дані між джерелом та S3](https://aws.amazon.com/about-aws/whats-new/2023/03/aws-database-migration-service-s3-data-validation/), so you don't have to ;)
- також, коли ви вибрали S3 sink даних, [DMS може автоматично творити запис у AWS Glue Catalog](https://aws.amazon.com/about-aws/whats-new/2023/03/aws-database-migration-service-aws-glue-data-catalog-amazon-s3/) для ваших даних. Це дасть змогу одразу через Athena здійснювати запити до даних.