# Criando máquinas virtuais

## 1. Localizar o serviço

O serviço está localizado na divisão Compute, com o nome de Virtual Machines ou Máquinas virtuais:
    ![image](https://github.com/pablof9610/dio-azure/blob/main/assets/image1.png)

## 2. Criar a máquina virtual

No menu Create, selecione Azure Virtual Machine:
![image](https://github.com/pablof9610/dio-azure/blob/main/assets/image2.png)

Em seguida, você pode escolher várias configurações e especificações do sistema operacional/hardware:
    ![image](https://github.com/pablof9610/dio-azure/blob/main/assets/image3.png)

É importante atentar para a configuração de portas abertas na máquina virtual. Por exmeplo, para acesso a uma VM Linux via SSH é importante que a porta 22 esteja aberta, assim como para o Windows a porta 3389 (RDP).

OBS: Caso não tenha uma faixa de subrede/IP público configurada, o Azure cria para você automaticamente.

## 3. Acessar a máquina
Existem muitas formas de acessar as máquinas. No caso do Linux, podemos utilizar o programa Putty ou Powershell para acessar via SSH (ssh usuario@meu_ip_publico), ou podemos utilizar o próprio CloudShell do Azure para conectar:
    ![image](https://github.com/pablof9610/dio-azure/blob/main/assets/image4.png)
    ![image](https://github.com/pablof9610/dio-azure/blob/main/assets/image5.png)
