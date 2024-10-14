# Identidade, acesso e segurança no Azure

O Azure também oferece serviços e recursos completos para gerenciar identidades, usuários, grupos e acessos e até segurança. Para o gerenciamento de usuário, temos o Microsoft Entra ID.

| Opção Entra ID | Descrição |
| ----- | --------- |
| Usuários | Aqui podemos gerenciar os usuários realizando operações como exclusão, atribuição de Roles e criação de usuários. É possível também criar novos usuários e também usuários externos. Também é possível verificar usuários que foram excluídos, os quais ficam em standby por até 30 dias disponíveis para restauração. |
| Funções e administradores | Cria e regula as Roles, necessárias para realizar o RBAC (Roled Based Access Control). |
| Nomes de domínio personalizados | Permite que administradores apliquem o domínio da empresa, os verificando e utilizando para identificar os usuários do entra ID. |

## RBAC
RBAC ou Roled Based Access Control é uma forma de conceder acesso a usuários e grupos a recursos específicos ou generalizados. Por exemplo, se for aplicado o RBAC a um resource group que contenha máquinas virtuais e VNETs, a permissão será herdada por todoso recursos dentro do mesmo. Algumas opções são:

| Opção | Descrição |
| ----- | --------- |
| Leitor | Exibe todos os recursos, mas não permite que você faça nenhuma alteração. |
| Admin de Segurança | Função do Admin de Segurança | 
| Administrador de Política de Serviços de Mídia | Crie, leia, modifique e exclua Filtros de Conta, Políticas de Streaming, Políticas de Chave de Conteúdo e Transformações; acesso somente leitura a outros recursos dos Serviços de Mídia. Não é possível criar recursos de Trabalhos, Ativos ou Streaming. |
| Administrador do Kubernetes do Azure Arc | Permite que você gerencie todos os recursos no cluster ou no namespace, exceto atualizar ou excluir as cotas de recursos e os namespaces. |

## Microsoft Entra Connect
Trabalha no meio de um ambiente On-Premises e um abiente de nuvem. Realiza a sincronização de usuários, grupos e outros que o administrador especificar. É interessante notar que um usuário que é criado no ambiente On-Premises é replicado para a nuvem através do Entra Connect, mas se um usuário é criado diretamente na nuvem, ele é chamado cloud-native e não é replicado para o ambiente físico.