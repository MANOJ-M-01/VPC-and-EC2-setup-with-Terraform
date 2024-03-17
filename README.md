# Steps
 - `terraform init`
 - `terraform plan`
 - `terraform apply`
 - `terraform destroy`

# Terraform apply Result

````sh
aws_vpc.my_test_vpc: Creating...
aws_vpc.my_test_vpc: Creation complete after 5s [id=vpc-XXXXXXXXXX]
aws_internet_gateway.my_ig: Creating...
aws_subnet.my_test_subnet: Creating...
aws_security_group.app_sg: Creating...
aws_subnet.my_test_subnet: Creation complete after 3s [id=subnet-XXXXXXXXXX]
aws_internet_gateway.my_ig: Creation complete after 4s [id=igw-XXXXXXXXXX]
aws_route_table.public_rt: Creating...
aws_route_table.public_rt: Creation complete after 3s [id=rtb-XXXXXXXXXX]
aws_route_table_association.public_1_rt_assoc: Creating...
aws_security_group.app_sg: Creation complete after 7s [id=sg-XXXXXXXXXX]
aws_instance.app_server: Creating...
aws_route_table_association.public_1_rt_assoc: Creation complete after 1s [id=rtbassoc-XXXXXXXXXX]
aws_instance.app_server: Still creating... [10s elapsed]
aws_instance.app_server: Still creating... [20s elapsed]
aws_instance.app_server: Still creating... [30s elapsed]
aws_instance.app_server: Still creating... [40s elapsed]
aws_instance.app_server: Creation complete after 47s [id=i-XXXXXXXXXX]

Apply complete! Resources: 7 added, 0 changed, 0 destroyed.

Outputs:

instance_id = "i-XXXXXXXXXX"
instance_public_ip = "XXXXXXXXXX"
````