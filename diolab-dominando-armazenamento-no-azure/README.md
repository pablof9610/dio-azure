# Armazenamento no Azure

Os serviços de armazenamento que o Azure oferece vão desde uma simples cópia para disponibilidade de arquivos de imagem para consumo frequente por uma aplicação web até a migração de uma aplicação, sistema ou até mesmo todos os dados de um datacenter para a nuvem.

## Storage Accounts
As Storage Accounts ou Contas de Armazenamento é um recurso do Azure que fornece armazenamento de arquivos, vídeos, GIFS, imagens, entre outros. Tudo na núvem e com fácil acesso. Existem algumas classificações de arquivos dependendo do propósito com o qual estão sendo armazenados.
Nas configurações de criação podemos especificar os arquivos entre:
- **Frenquente:** É cobrado mais pelo armazenamento e menos pelo acesso.
- **Esporádico:** É cobrado bem menos pelo armazenamento e mais pelo acesso.
- **Frio:** É cobrado muito menos pelo armazenamento e bem mais pelo acesso.
- **Arquivo Morto:** É cobrado muito menos pelo armazenamento e muito mais pelo acesso.

Também nas configurações podemos definir o modelo de dados da Conta de Armazenamento entre:
- **Blob:** É otimizado para armazenamento de quantidades massivas de dados não estruturados, como texto ou dados binários.É o modelo mais utilizado pelas aplicações, pois permite armazenar vídeos, fotos, GIF.
- **Queues (ou filas):** Serviço de armazenamento de mensagens que fornece armazenamento e recuperação para grandes quantidades de mensagens, cada uma com até 64 KB.
- **Tables (ou tabelas):** Fornece uma opção de chave/atributo para armazenamento de dados estruturados não relacionais com um design em schema.
- **File Shares:** Configura um compartilhamento de arquivos de rede altamente disponível que pode ser utilizado usando o protocolo Bloco de Mensagens do Servidor. _Detalhe: Pode ser acessado através do protocolo SMB (porta 445)_

## AzCopy

É ideal quando houver a necessidade de mover dados para a núvem e não se encaixar no cenário de utilizar um serviço como o Azure Data Box. Fornece benefícios como:

- Utilitário de linha de comando;
- Ajuda a copiar blobs ou arquivos de ou para uma conta de armazenamento.
- Sincronização em uma direção.
- Pode ser utilizado no Windows, MacOS e Linux.

## Azure Databox

É uma solução adequada para migração/movimentações de dados, sendo aconselhável utilizar acima de 60 TB. Características:

- Consegue carregar até 80 TB de dados;
- Move os backups de recuperação de desastre para o Azure;
- Proteja seus dados em uma caixa robusta durante o trânsito;
- Migra os dados do Azure por conformidade ou necessidades regulatórias;
- Migra os dados para o Azure, sendo mais proveitoso onde há cenários de locais remotos com conectividade limitada ou sem conectividade.