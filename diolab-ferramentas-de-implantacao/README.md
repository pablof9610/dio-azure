# Ferramentas de Implantação

O Azure também oferece incríveis ferramentas para interação com o ambiente Cloud de várias maneiras, como:

- **Portal do Azure:** Portal simplificado onde podemos gerenciar, criar, excluir e modificar recursos de forma eficiente.
- **Azure PowerShell:** Cria uma sessão de PowerShell onde é possível interagir com o ambiente dentro da Azure.
- **Azure Cloud Shell:** Faz o mesmo que o PowerShell, porém o diferencial é que cria no estilo bash.
- **Interface de Linha de Comando (CLI):** Interface de linha de comando para interagir com o ambiente da Azure.

## Azure Arc

É uma ferramenta dos moldes de multicloud. Serve para que façamos o gerenciamento de recursos que não estão dentro do Azure. 

Por exemplo: Em um cenário onde temos uma assinatura com a microsoft e um ambiente on-premises onde há uma dificuldade de fazer um gerenciamento separado. Podemos adicionar um script em máquinas no ambiente on-premises e começarão a aparecer no módulo do Arc no painel da microsoft. Essa técnica também pode ser utilizada tanto no AWS como no GCP.

## Azure Resource Manager (ARM)

O ARM (Azure Resource Manager) fornece uma camada de gerenciamento que permite criar, atualizar e excluir recursos na assinatura do Azure. Funciona como um centralizador de requisições feitas para o Azure, criando e alterando os recursos de acordo com os templates existentes.