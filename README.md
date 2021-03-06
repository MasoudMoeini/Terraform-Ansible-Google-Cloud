# Terraform Ansible Google Cloud
[Reference](https://github.com/antonputra/tutorials/tree/main/lessons/101)<br/>
Integration of terraform with ansible to provide Iaac in Google Cloud <br/>
Milestones: <br/>
- Generating ssh key pair 
```
ssh-keygen -t ed25519 -f ~/.ssh/ansbile_ed25519 -C ansible
```
```
cat ~/.ssh/ansbile_ed25519.pub
``` 
- Config Compute engine with ssh key<br/>
```
terraform init
```
```
terraform plan 
```
```
terraform apply 
```
Terraform prints the VM's external IP address and port 80 has been set in firewall configuration to access vm<br/>
Web-server-URL(nginx_ip:80):<br/>
```
http://IP_ADDRESS:80
```
At any time to acces ip address by:
```
terraform output
```
You should see something similar in browser:<br/>
<img width="901" alt="Screenshot 2022-07-13 at 11 01 38" src="https://user-images.githubusercontent.com/43514418/178695362-f0f983fd-5d24-416d-bdb3-9feba0744502.png"><br/>

To remove resources:
```
terraform destroy
```
```
rm ~/.ssh/ansbile*
```
Delete SSH public key from GCP project




