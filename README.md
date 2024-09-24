# aws-vpc-eks
1. 1 VPC, 2 public subnets and 6 private subnets, and 1 Internet Gateway and NAT Gateway via cf_basic_infra.yaml.

2. create-ekcluster.yaml is a template for deploying EKS clusters, which deploys the cf_basic_infra.yaml template in advance, adds the corresponding ID value, and deploys one EKS cluster.
