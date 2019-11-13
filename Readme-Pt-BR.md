Code Versioning Standard (CVS)
===

O  Code Versioning Standard (CVS) foi desenvolvido para oferecer suporte a projetos **GIT** ou **SVN** para que haja maior organização dos arquivos que são versionados no repositório. Devemos inserir comentários precedidos pelas ações que foram executadas nos arquivos versionados. Dessa maneira o versionamento de código-fonte fica mais flexivel e coeso, facilitando a identificação do que foi realizado. 

## Como utilizar

Como padrão, cada ação deve ser colocada entre colchetes precedido do que foi realizado de forma clara e objetiva durante o versionamento do código. 

## Ações

As opções abaixo representam opções que podem ser usadas no início de cada confirmação.

| Ações    | Descrição |
|:-:       |:-: |
|[ADD]     | Usado para quando os arquivos são adicionados ao projeto |
|[REMOVE]  | Usado para sinalizar remoção de arquivos |
|[MOVE]    | Usado quando um arquivo é movido de um diretório para outro.|
|[UPDATE]  | Usado para aprimorar um arquivo existente |
|[REFATOR] | Usado para refatoração de código fonte |
|[PATCH]   | Usado para representar rotinas para correções temporárias.
|[FIX]     | Utilizado para representar a correção de erros / falhas, identificada pelo gerente ou equipe que trabalha no código-fonte |
|[MERGE]   | Usado quando a mesclagem de arquivos é executada |
|[RENAME]  | Usado quando um arquivo é renomeado. |

## Uso

### Mensagem padrão
```
[ADD] Definição de arquivos xyz
```

### Título e descrição
```
[UPDATE] Pagamento usando cartões

Criação de funcionalidade que permite efetuar pagamentos usando o cartão de crédito com bandeira XPTO.
```

### Mensagens em Módulos

Caso sejam utilizados **módulos** e **funcionalidades**, utilize o padrão `[acao] módulo/funcionalidade: ` precedidos de uma breve descrição.
```
[FIX] NomeDoMódulo/Funcionalidade: Descrição

Descrevendo o que foi feito nessa correção.
```

## Como NÃO usar

Não é uma boa prática agrupar várias ações no mesmo commit. É recomendável que as confirmações sejam vinculadas à ação.

```
[UPDATE/FIX] Descrição da alteração e correção.
```

## Idiomas
- [EN](./README.md)
