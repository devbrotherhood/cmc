Commit Messages Convention (CMC)
===

O  Commit Messages Convention (CMC) foi desenvolvido para oferecer suporte a projetos **GIT** ou **SVN** para que haja maior organização dos _commits_ no repositório.
Ela define que a inserção de comentários deve ser precedido pelos tipos de ações que foram executadas nos arquivos versionados.
Dessa maneira o versionamento de código-fonte fica mais flexível e coeso, facilitando a identificação do que foi realizado.
Esta convenção segue o [SemVer](http://semver.org/), descrevendo os recursos, correções e modificações que quebram a compatibilidade nas mensagens de _commit_. 

## Especificação
As palavras-chaves "MUST" (DEVE), "MUST NOT" (NÃO DEVE), "REQUIRED" (OBRIGATÓRIO), "SHALL" (DEVERÁ), "SHALL NOT" (NÃO DEVERÁ), "SHOULD" (PODEM), "SHOULD NOT" (NÃO PODEM), "RECOMMENDED" (RECOMENDADO), "MAY" (PODE) e "OPTIONAL" (OPCIONAL), nesse documento, devem ser interpretados como descrito na [RFC 2119](http://tools.ietf.org/html/rfc2119).

## Como utilizar

Como padrão, cada tipo DEVE ser colocado com letra maiúscula, entre colchetes, precedendo o que foi realizado de forma clara e objetiva durante o versionamento do código.

A mensagem de _commit_ DEVE ser estruturada da seguinte forma:

```
[TIPO obrigatório] <descrição|cabeçalho obrigatório>
--linha em branco--
<corpo opcional>
--linha em branco--
<rodapé opcional>
```
##### A mensagen:
- DEVE iniciar com um [TIPO]
- O [TIPO] DEVE ser com letras maiúsculas, entre colchetes, seguido por um espaço
- DEVE conter uma <descrição> apos o [TIPO]
- PODE conter um <corpo> e/ou <rodapé>
- DEVE conter uma --linha em branco-- apos a <descrição> caso tenha <corpo>
- DEVE conter uma --linha em branco-- apos a <corpo> caso tenha <rodapé>

### Tipos

Os tipos abaixo representam opções que podem ser usadas no início de cada _commit_.

| Tipo      | Descrição |
|:-:        | :-: |
|[FEAT]     | Quando um novo recurso foi desenvolvido |
|[FIX]      | Quando um recurso/bug foi corrigido |
|[UPDATE]   | Quando arquivos estáticos foram renomeados, removidos, movidos de um diretório para outro, adicionados ou substituídos |
|[REFACTOR] | Quando uma alteração de código que não corrige um bug nem adiciona um recurso |
|[DOCS]     | Somente alterações na documentação |

### Tipos especiais

É RECOMENDADO que os tipos especiais sejam utilizados em conjunto com os tipos anteriores, porem, eles PODEM ser usados em qualquer parte da mensagem.

| Tipo                              | Descrição |
|:-:                                | :-: |
|[WIP]                              | Quando um desenvolvimento ainda esta em progresso |
|[BREAKING] ou [BREAKING CHANGE]    | Quando o _commit_ inclui uma modificação que quebra a compatibilidade. PODE ser usado em qualquer parte do _commit_ (<descrição>, <corpo> ou <rodapé>) |

#### Exemplos:
```
[FEAT][WIP] Introduz um novo método de pagamento
```
```
[FIX][BREAKING] Substitui o gateway do PagSeguro por PayPal
```

### Descrição

Para a mensagem de <descrição> e do <corpo> do _commit_, faz-se o uso do padrao ["Commit Message Guide"](https://github.com/RomuloOliveira/commit-messages-guide/blob/master/README_pt-BR.md) do @RomuloOliveira, que basicamente consiste em:
- **Usar o imperativo**: A mensagem de _commit_ diz o que ele faz, não o que foi **feito**.
- **Primeira letra em maiúsculo**: porque é assim que se começa uma frase em qualquer texto.
- **Tente comunicar o que o _commit_ faz sem que seja necessário olhar o conteúdo do _commit_.**

### Corpo

- **Use o corpo da mensagem para explicar "porquê", "para quê", "como" e detalhes adicionais.**
- **Evite _commits_ com mensagens genéricas ou sem contexto algum.**
- **Tente limitar o nº de colunas das mensagens:** Recomenda-se 50 caracteres para a <descrição> e por volta de 72 para o <corpo>.
- **Mantenha consistência de idioma:** Escolha um idioma e mantenha-se nele.

### Rodapé

Um <rodapé> de uma ou mais linhas PODE ser fornecido depois de uma --linha em branco-- após o <corpo>.
O <rodapé> DEVE conter informações adicionais sobre o _commit_, por exemplo, numero da issue/task, pull-requests, revisores, modificações que quebram a compatibilidade, com uma informação adicional por linha.

## Exemplos
```
[FIX] Corrige a chamada do método "getProducts"

O retorno esperado do método "getProducts" era um array, porem retornava um objeto, isso causava um erro em produção.

Corrige a issue #92
```

```
[FEAT][WIP] Cria a classe PayPalGateway

Cria a estrutura base da integração com PayPal, assim como a interface de Gateway para uso futuro.
```

```
[REFACTOR] Refatora a classe PagSeguro

Reescrita da class PagSeguroGateway, para se adequar ao padrao da interface Gateway.
[BREAKING CHANGE] Como a classe PagSeguroGateway foi refatorada, todos os método também foram modificados.

Depende do commit sd5f54s
```

```
[UPDATE] Adiciona os arquivos CSS e images

Adiciona os arquivos que estavam faltando no diretório assets/
```

## Idiomas
- [EN](./README.md)

## Referências
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)
- [Conventional Commits](https://www.conventionalcommits.org/pt-br/)
- [Commit Messages Guide](https://github.com/RomuloOliveira/commit-messages-guide)
- [Angular Commit Message Guidelines](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)
