Нещодавно у блозі Uber був цікавий пост про міграцію Hadoop з чистого заліза на контейнери. Цього разу AWS [опублікував](https://aws.amazon.com/blogs/big-data/run-and-debug-apache-spark-applications-on-aws-with-amazon-emr-on-amazon-eks/) покроковий посібник як запустити Spark аплікацію використовуючи EMR на Kubernetes(а точніше на EKS). 

Як на мене користь сумнівна. K8s - технолгія непроста, так само як і Hadoop. Міксування одного з іншим може обернутись сотнями годин відлагодження інфраструктури. 
З плюсів - економія грошей та уніфікація, але знову ж таки, при умові що EMR на EKS буде працювати без проблем(в що мало віриться). 