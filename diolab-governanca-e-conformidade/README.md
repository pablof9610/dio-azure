# Governança e conformidade no Azure

O Azure oferece ótimas ferramentas de controle de segurança, conformidade e de governança. Uma delas é o Azure Policy, que é como uma autoridade maior que qualquer permissão de usuário. Elas ajudam a impor padrões organizacionais e a avaliar a conformidade em escala. Se uma Policy define que recursos não serão criados em determinada região, não serão, mesmo se usuários com as mais elevadas permissões tentarem. Ele oferece algumas opções de estados de recursos, como:

| Opção | Descrição |
| ----- | --------- |
| Non-Compliant | Se por exemplo definirmos que um recurso é criado somente no Brasil. Caso qualquer usuário crie em outro país surgirá um alerta de Non-compliant.|
| Remendiation | Se um recurso que está sendo criado ou que já foi, a policy irá mostrar como remendation, ou seja, como necessário alterações. |
| Compliant | Todos os itens que respondem para aquela Policy estão seguindo os padrões esperados. |

Outra ferramenta importante é o Bloqueio de Recurso. Porém é importante entender o que se está fazendo ao criar um bloqueio, devemos tomar cuidado e observar o contexto, pois ao bloquear a exclusão em um grupo de recursos, por exemplo, se algum recurso como uma máquina virtual criar para fazer um backup criar uma cópia fantasma ou fictícia e no final da rotina de backup tentar excluir a cópia, não conseguirá excluir, o que gerará mais custo.

Existem dois tipos de bloqueios, são eles:

## Excluir:
| Ler | Atualizar | Excluir |
| ----- | --------- | --------- |
| Sim | Sim | Não |

## Somente leitura:
| Ler | Atualizar | Excluir |
| ----- | --------- | --------- |
| Sim | Não | Não |