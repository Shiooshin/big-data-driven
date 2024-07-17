AWS в своєму блозі написала [чому вам варто перенести свій EMR кластер на Kubernetes(EKS)](https://aws.amazon.com/blogs/big-data/amazon-emr-on-amazon-eks-provides-up-to-61-lower-costs-and-up-to-68-performance-improvement-for-spark-workloads/). Головними факторами переходу AWS називає зменшення витрат на кластер та збільшення продуктивності. Проте сама стаття може ввести вас в оману, якщо не читати уважно. AWS насправді пише, що AWS EMR на EKS дешевший і швидший **в порівнянні з Open-source Spark**, який ви руками будете піднімати на EKS. Навіть глянувши на тести, EMR на EC2 не набагато поступається у швидкодії того ж EMR на EKS. Тому немає потреби гасити ваш існуючий кластер і поспіхом підіймати такий же, тільки на EKS. Але якщо ціна вашого кластера вам здається завеликою - то контейнери будуть дешевші ніж віртуалки і гнучкііші в управлінні ресурами.

Ще рік тому використання Hadoop дистрибутивів на Kubernetes виглядало сирим і проблемним рішенням. Проте навіть хмарні провайдери активно рухались у цьому напрямку і, як бачимо, вже є можливість спробувати наскільки ефективним буде обробка великих масивів даних на Kubernets. Я б точно перевіврив, якби була потреба, але ми майже всюди використовуємо AWS Glue для обробки даних, а не EMR.