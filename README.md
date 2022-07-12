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
To remove resources:
```
terraform destroy
```
```
rm ~/.ssh/ansbile*
```
Delete SSH public key from GCP project




