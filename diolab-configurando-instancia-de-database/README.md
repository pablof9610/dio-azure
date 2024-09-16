# Azure SQL Database

O SQL Database do Azure é uma ferramenta poderosa pois oferece uma solução de banco de dados em núvem, ela oferece disponibilidade, segurança e flexibilidade para acesso aos dados.

## Configuração

Também oferece uma grande flexibilidade para conexão. Dentre algumas configurações, estão:

| Configuração | Descrição |
| ------ | ------ |
| Regra de Firewall (Acesso Público) | É possível configurar regras adicionando nomes e ranges de IP para apenas determinadas faixas de IP se conectarem ao servidor e as demais não. |
| Acesso privado | É possível configurar endpoints privados de uma rede virtual que já existe dentro da Azure. |
| Configuração de Portas | Podemos também liberar e bloquear portas como a 1433 para que o SQL Database funcione corretamente. |
| Política de Conexão | Dentre as políticas de conexão podemos configurar entre Default, Proxy e Redirect quando falamos acerca de conexões de fora da nuvem. |
| Segurança | É possível realizar configurações como versão mínima do protocolo TLS do servidor, meio de autenticação para acesso.

## GUI para modelar o banco

Existe uma ferramenta chamada Query Editor que nos permite executar instruções SQL dentro do banco que criamos. Para acessar, é necessário informar as credenciais em conformidade com a forma de autenticação configurada.