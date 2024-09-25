# Configuração de Recursos

## Dimensionamento em Máquinas Virtuais

Nas configurações da aba Básico nas estapas de criação de uma máquina virtual é possível selecionar a opção de disponibilidade da máquina virtual. Dentre as opções, temos:

| Opção | Descrição |
| ----- | --------- |
| Zona de disponibilidade | Proporciona uma separação física dos recursos pelas regiões do Azure. |
| Conjunto de disponibilidade | Permite criar domínios de falha (Que são Racks) e domínos de atualização, que são VMs programadas para assumir o controle caso outras demais fiquem inoperantes. |
| Conjunto de dimensionamento de máquinas virtuais | Semelhante ao Conjunto de Disponibilidade, porém oferece configurações de escala automática, onde condições configuradas para, por exemplo, medir o consumo da CPU cria novas instâncias da máquina virtual.

É interessante saber que ao criar um novo conjunto de dimensionamento de máquinas virtuais é possível escalar os recursos horizontalmente.

Em modo de dimensionamento, temos:
- **Atualizar manualmente a capacidade:** Mantém uma quantidade fixa de instâncias.
- **Dimensionamento automático:** Dimensiona com base em uma métrica de CPU, por exemplo: Toda vez que a CPU atingir 80% de utilização, serão criadas **n** novas instâncias de acordo com o especificado na condição de dimensionamento.
- **Sem perfil de colocação em escala:** Aumentar ou diminuir máquinas virtuais manualmente após a implantação.

## Azure Functions

A Azure Functions é um ótimo recurso para um cenário onde é necessário executar alguma função de um código quando um evento acontecer. Dentre as várias configurações, temos:

- **Pilha de Runtime:** Aqui especificamos a linguagem que será rodada e compilada na Function criada. Podendo ser .NET, Node.js, Python, Java, Powershell Core ou Custom Handler.
- **Versão:** Oferece uma personalização da versão da linguagem utilizada, com todas as suas features referentes a cada versão.
- **Região:** Aloca fisicamente a Function ao redor das áreas de disponibilidade do Azure.
- **Sistema Operacional:** Sistema Operacional que irá hospedar a função.
*OBS:* Dependendo da Pilha de Runtime (ou linguagem) pré-configurada o Sistema Operacional pode mudar, sendo apenas a linguagem Python disponível no Linux.