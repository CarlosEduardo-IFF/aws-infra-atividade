# aws-infra-atividade

## 1 - Criação de Security Groups (Grupos de Segurança):

### a - Security Group para EC2:

* Acesse o AWS Console > EC2 > Security Groups;
* Clique em "Create security group":
  
  ![Security Group](imgs/security-groups/create_1.PNG)

* Adicione "Security group name" e "Description":

  ![Security Group](imgs/security-groups/namedescEC2.PNG)

* Adicione as regras para liberar acesso SSH (porta 22) para o IP pessoal e para liberar acesso HTTP (porta 80) ou Custom para qualquer IP(0.0.0.0/0):

   ![Security Group](imgs/security-groups/ssh_http.PNG)

* Clique em "Create security group" para criar:

  ![Security Group](imgs/security-groups/create_1_end.PNG)

* Após a criação, aparecerá que o security group foi criado com sucesso:

  ![Security Group](imgs/security-groups/sg_ec2_criado.png)


### b - Security Group para RDS:

* Acesse o AWS Console > EC2 > Security Groups;
* Clique em "Create security group":
  
  ![Security Group](imgs/security-groups/create_2.PNG)

* Adicione "Security group name" e "Description":

  ![Security Group](imgs/security-groups/namedescRDS.PNG)

* Adicione a regra para permitir conexão PostgreSQL (porta 5432) apenas para o Security Group da EC2 criado anteriormente:

   ![Security Group](imgs/security-groups/rds.PNG)

* Clique em "Create security group" para criar:

  ![Security Group](imgs/security-groups/create_2_end.PNG)

* Após a criação, aparecerá que o security group foi criado com sucesso:

  ![Security Group](imgs/security-groups/sg_rds_criado.png)


## 2 - Criar uma Instância EC2:

* Acesse AWS Console > EC2 > Instances;
* Clique em "Launch Instances":

  ![EC2](imgs/ec2/create.PNG)

  
  

