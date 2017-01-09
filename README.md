PVC( Padrão de versionamento de código )
===


Para que haja maior organização dos arquivos que são versionados no repositório, devemos inserir comentários precedidos pelas ações que foram executadas nos arquivos versionados. Portanto, decidi criar um padrão de versionamento de código para que fique mais flexivel identificar o que foi realizado nos commits. 

===
Como padrão, deve ser colocado entre coxetes e caixa alta, o tipo de ação utilizada para versionar um ou mais arquivos, podendo ser utilizada mais de uma ação no versionamento do código e logo após um breve comentário do que foi realizado. 

Lista de ações adotar o padrão abaixo: 

* [ADD] ­ Adição de novos arquivos no projeto;

* [REMOVE] ­ Utilizado para sinalizar a remoção de arquivos;

* [MOVE] ­ Utilizado quando algum arquivo é movido de um diretório para outro.

* [UPDATE] ­ Melhoria de um arquivo já existente;

* [REFACTOR] ­ Refatoração de código-fonte

* [BACKUP] Funcionalidade incompleta, mas para garantir a segurança e reusa
bilidade de código-­fonte por outros membros da equipe;

* [PATH] ­ Correção de um erro/falha, identificado pela equipe que está trabalhando no código-fonte;

* [FIX] ­ Correção de um erro/falha, identificada pelo gestor;

* [MERGE] ­ Utilizado quando é realizado o merge de arquivos;

* [RENAME] ­ Utilizado quando um arquivo é renomeado.

* [LOCK] Utilizado quando é aplicado um lock em um arquivo.


 
Exemplos
===

* Exemplo 1: [UPDATE] Refatoração da classe. 

* Exemplo 2: [ADD/UPDATE/MOVE] Descrição do que foi realizado em um ou mais arquivos. 
