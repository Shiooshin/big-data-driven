AWS Grafana is billed per user per workplace. All user licenses are per workspace, per month. Each workspace requires a minimum of one Amazon Managed Grafana Editor license in order to manage and log into the workspace, even if no users log in. An Amazon Managed Grafana Editor license costs $9 per active editor or administrator user per workspace. An Amazon Managed Grafana Viewer license costs $5 per active user per workspace and provides the user with view-only access to the Amazon Managed Grafana workspace

Amazon Managed Grafana will offer a 90-day free trial, with up to five free users per account



EC2 Grafana
launch EC2
https://docs.aws.amazon.com/AmazonECS/latest/developerguide/docker-basics.html
https://grafana.com/docs/grafana/latest/installation/docker/
https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html#WorkingWithSecurityGroups to allow 3000 port for Internet

configure CloudWatch
https://grafana.com/docs/grafana/latest/datasources/aws-cloudwatch/aws-authentication/
https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html

EC2 micro for Grafana:
us-east-1 + 50Gb SSD storage + Reserved for 1 year(No Upfront) + 24/7 instance time = 10.26 USD/month

managed Grafana
Easy to set up BUT needs additional SSO + Organization
AWS Services data source out of box
Has different set of metrics
90-days free to try
Has locked Grafana version  