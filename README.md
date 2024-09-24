# aws-vpc-eks
1. 1 VPC, 2 Public subnets and 6 Private subnets(Frontend(2), Backend(2), Database(2)), and 1 Internet Gateway and NAT Gateway via cf_basic_infra.yaml.

2. create-ekcluster.yaml is a template for deploying EKS clusters, which deploys the cf_basic_infra.yaml template in advance, adds the corresponding ID value, and deploys one EKS cluster.

3. Public Subnet has 8,192 IPs, Private Subnet has 8,192 IPs for Frontend, 8,192 IPs for Backend, and 2,048 IPs for Database.

Notification
ETEVERS-IDE is a code server and configures a pre-created IAM
