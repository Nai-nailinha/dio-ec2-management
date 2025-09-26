# 🚀 Gerenciamento de Instâncias EC2 na AWS  

## 📌 Sobre este repositório  
Este repositório foi criado como parte do desafio da [DIO](https://web.dio.me/) no bootcamp **Santander Code Girls AWS**.  
Aqui estão reunidas minhas anotações e insights do laboratório de **Gerenciamento de Instâncias EC2**.  

## 🎯 Objetivos do Desafio  
- Aplicar os conceitos aprendidos sobre **EC2** em um ambiente prático.  
- Documentar processos técnicos de forma clara e organizada.  
- Utilizar o GitHub como vitrine do aprendizado e material de consulta futura.  

## 🖥️ Passo a Passo realizado  

### 1. Criando a instância  
- Escolhi a AMI: (ex.: Amazon Linux 2, Ubuntu…).  
- Tipo da instância: (ex.: t2.micro – dentro do Free Tier).  
- Par de chaves SSH: criado e baixado com segurança.  

### 2. Configuração de rede e segurança  
- VPC: (ex.: default).  
- Subnet: (ex.: us-east-1a).  
- Security Group: liberadas portas **22 (SSH)**, **80 (HTTP)** e **443 (HTTPS)**.  

### 3. Conectando na instância  
- Método usado: (ex.: EC2 Instance Connect, SSH via terminal).  
- Comandos básicos executados:  
  ```bash
  sudo yum update -y
  ```

### 4. Parando e iniciando a instância  
- Experimentei parar a instância e reiniciar → dados preservados no EBS.  
- Observação: instância parada não gera custo de computação, mas o **EBS continua sendo cobrado**.  

### 5. Encerrando a instância  
- Encerrada para liberar recursos.  
- Observação: após o encerramento, o IP público foi perdido.  

## 📈 Insights pessoais  
- ⚡ Elasticidade: é prático escalar para tipos maiores de instância em minutos.  
- 🔐 Segurança: *Security Groups* funcionam como o “porteiro” da instância: só entra quem eu deixar.  
- 💸 Custos: importante configurar **Billing Alarms** para evitar surpresas.  


## 🖼️ Evidências (prints)  
Imagens do laboratório estão organizadas na pasta `/images`. Exemplos:  
- Criação da instância.  
- Configuração do Security Group.  
- Conexão via SSH.  


## 📚 Referências  
- [Documentação AWS – Amazon EC2](https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/concepts.html)  
- [GitHub Docs – Guia de Markdown](https://docs.github.com/pt/github/writing-on-github/basic-writing-and-formatting-syntax)  


✨ Desafio concluído com sucesso!  
Esse repositório vai servir como **material de apoio para estudos futuros** e também como vitrine do meu aprendizado em **Cloud AWS**.  
