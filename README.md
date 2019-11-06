PVC
===

## Significado

PVC significa Padrão de versionamento de código.

## Sobre
Para que haja maior organização dos arquivos que são versionados no repositório, devemos inserir comentários precedidos pelas ações que foram executadas nos arquivos versionados. Dessa maneira o versionamento de código-fonte fica mais flexivel e coeso, facilitando a identificação do que foi realizado. 

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

## Como utilizar
Como padrão, deve ser colocado entre colchetes e caixa alta, o tipo de ação utilizada para versionar os arquivos, podendo ser utilizada mais de uma ação no versionamento do código. Após, caso se aplique, indique o módulo / funcionalidade e dois pontos; por último, descreva num breve comentário o que foi realizado. 

## Formas de utilização

### Mensagem Padrão
```
[ ADD ] Definição de arquivos xyz
```

### Titulo e descrição
```
[ UPDATE ] Pagamento utilizando cartões

Criação de funcionalidade que permite realizar pagamentos utilizando o cartão de crédito da bandeira XPTO.
```

### Mensagens por módulos 
```
[ FIX ] Módulo/nome_funcionalidade

Descrevendo o que foi feito nessa correção.
```

### Agrupamento de ações
```
[UPDATE/FIX] Descrição da alteração e correção.
``` 
