PVC
===

## Significado

PVC significa Padrão de versionamento de código.

## Sobre
Para que haja maior organização dos arquivos que são versionados no repositório, devemos inserir comentários precedidos pelas ações que foram executadas nos arquivos versionados. Dessa maneira o versionamento de código-fonte fica mais flexivel e coeso, facilitando a identificação do que foi realizado. 

## Como utilizar
Como padrão, deve ser colocado entre colchetes e caixa alta, o tipo de ação utilizada para versionar os arquivos, podendo ser utilizada mais de uma ação no versionamento do código. Após, caso se aplique, indique o módulo / funcionalidade e dois pontos; por último, descreva num breve comentário o que foi realizado. 

Exemplos:

    [ FIX ] Módulo/nome_funcionalidade: descrição da alteração
    [ UPDATE ] Descrição da alteração
    [ ADD ] [ FIX ] Descrição da alteração   


## Lista de ações e suas respectivas funções 

#### [ ADD ] 
```
 Utilizado para quando arquivos são adicionados no projeto;
```
#### [ REMOVE ]
```
 Utilizado para sinalizar a remoção de arquivos;
```
#### [ MOVE ]
```
 Utilizado quando algum arquivo é movido de um diretório para outro.
```
#### [ UPDATE ]
```
 Utilizado para melhoria de um arquivo já existente;
```
#### [ REFACTOR ]
```
 Utilizado para refatoração de código-fonte
```
#### [ PATCH ]
```
 Utilizado para representar rotinas de para correções temporárias.
```
#### [ FIX ]
```
 Utilizado para representar Correção de um erro/falha, identificada pelo gestor ou equipe que está trabalhando no código-fonte;
```
#### [ MERGE ]
```
 Utilizado quando é realizado o merge de arquivos;
```
#### [ RENAME ]
```
 Utilizado quando um arquivo é renomeado.
```
#### [ REWORK ]
```
 Utilizado quando há retrabalho
```

## Exemplos

#### Exemplo 1: 
```
[ ADD ] Adicionados módulo para realizar transações bancárias
[ UPDATE ] Criação de funcionalidade que permite realizar pagamentos utilizando o cartão de crédito da bandeira XPTO.
[ MOVE ] Classes que não faziam parte do escopo das transações bancárias foram movidas para seus respectivos módulos
```
#### Exemplo 2: 
```
[ REFACTOR ] Refatoração da classe XPTO para que fique mais coesa.
[ MERGE ] Merge da branch feature-album com a branch develop
```
