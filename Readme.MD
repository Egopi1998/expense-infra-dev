for i in 01-vpc/ 02-sg/ 03-bastion/ 04-db/ 05-vpn/ 06-app-alb/ 07-backend/ 08-acm/ 09-web-alb/ 10-frontend/ 11-cdn/; do cd $i ; terraform init; terraform apply -auto-approve; cd ..; done

for i in 11-cdn/ 10-frontend/ 09-web-alb/ 08-acm/ 07-backend/ 06-app-alb/ 05-vpn/ 04-db/ 03-bastion/ 02-sg/ 01-vpc/; do cd $i; terraform destroy -auto-approve; cd ..; done

terraform init

terraform plan

terraform apply -auto-approve

terraform destroy -auto-approve

for i in 07-backend/ 06-app-alb/ 05-vpn/ 04-db/ 02-sg/ 01-vpc/; do cd $i; terraform destroy -auto-approve; cd ..; done

for i in 10-frontend/; do cd $i ; terraform init; terraform apply -auto-approve; cd ..; done

for i in 08-acm/ 09-web-alb/ 10-frontend/; do cd $i ; terraform init; terraform apply -auto-approve; cd ..; done