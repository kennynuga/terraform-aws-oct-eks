<<<<<<< HEAD
# eks-module
=======
# MY AWESOME TERRAFORM MODULE TO PROVISION EKS CLUSTER WITH CUSTOM NETWORKING  ----->

# Sample usage:

~~~ 

module "oct-eks" {
  source         = "github.com/kennynuga/oct-eks.git"
  region         = "eu-west-2"
  vpc_cidr       = "10.0.0.0/16"
  dns_hostnames  = true
  dns_support    = true
  pub_one_cidr   = "10.0.1.0/24"
  pub_two_cidr   = "10.0.2.0/24"
  priv_one_cidr  = "10.0.3.0/24"
  priv_two_cidr  = "10.0.4.0/24"
  az_one         = "eu-west-2a"
  az_two         = "eu-west-2b"
  vpc_id         = "aws_vpc.eks_vpc.id"
  eks_version    = "1.26"
  ami_type       = "AL2_x86_64"
  instance_types = ["t3.small", "t3.medium", "t3.large"]
  capacity_type  = "ON_DEMAND"

}

~~~

 ----- end of readme file -----
>>>>>>> d9de89f (new commit)
