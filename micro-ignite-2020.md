Сьогодні почалась інженерна конференція [Ignite 2022](https://ignite.microsoft.com/en-US/sessions), яку хостить компанія Microsoft. Сесії всі мають теги, а отже можна пофільтрувати як вам завгодно. На конференції буде аж 60 сесій стосовно інженерії даних на Azure Cloud. Можна знайти щось, що може вас зацікавити, яки ви працюєте з Azure чи з PowerBI.


gcloud compute instance-templates create lb-backend-template \
   --region= \
   --network=default \
   --subnet=default \
   --tags=allow-health-check \
   --machine-type=e2-medium \
   --image-family=debian-11 \
   --image-project=debian-cloud \
   --metadata=startup-script='cat << EOF > startup.sh
#! /bin/bash
apt-get update
apt-get install -y nginx
service nginx start
sed -i -- \'s/nginx/Google Cloud Platform - '"\\$HOSTNAME"\'/' /var/www/html/index.nginx-debian.html
EOF'