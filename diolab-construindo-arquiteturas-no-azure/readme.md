# Criando Grupos de Recursos

Os grupos de recursos oferecem vários benefícios pois podem agrupar e centralizar vários recursos de forma personalizada, de acordo com a necessidade.

Existem algumas funcionalidades que estão disponíveis para uso dentro de um grupo de recursos:

| Opção | Descrição |
| ------- | --------- |
| Log de Atividades | Esta funcionalidade é útil quando a intenção é verificar quais mudanças foram feitas, o que foi adicionado e quando. Serve como um tipo de auditoria. |
| Bloqueios | Como o nome já diz, define regras dentro daquele grupo de recursos para evitar exclusões ou alterações acidentais. Possui duas opções, sendo Apenas-Leita e Exclusão. |
| Implantações | Mostra o que já foi implantado naquele grupo de recursos, como a criação de uma Rede Virtual que no momento da criação foi atribuída àquele grupo de recursos. |
| Visualizador de Recursos | À medida que os recursos vão sendo criados, esta funcionalidade cria uma árvore que mostra de forma gráfica todos os recursos que estão dentro daquele grupo. |
| Controle de Acesso (IAM) | Aqui é possível controlar o acesso dos usuário somente a este grupo de recurso e aos recursos dentro dele.

Como exemplo, podemos criar um grupo de recurso para máquinas virtuais, e outro dedicado aos discos dessas máquinas. Também é possível atribuir Tags ou Marcações para que a organização seja completa, até mesmo quando aqueles recursos forem cobrados. Dessa forma, todo o gerenciamento dos recursos ficaria mais simplificado e organizado, pois se poderia medir o custo que determinado grupo de recurso está gerando, além de identificá-lo de forma mais fácil por conta das Tags.