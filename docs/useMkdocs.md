---
## Guia Detalhado para Escrita de Documentação no MkDocs

Este guia oferece uma explicação detalhada de como escrever sua documentação utilizando o MkDocs, cobrindo desde a estrutura básica até elementos mais avançados como formatação de texto, links e inclusão de código.

---

### Estrutura Básica de um Arquivo Markdown

O MkDocs utiliza **Markdown** para escrever o conteúdo da sua documentação. Markdown é uma linguagem de marcação leve que permite formatar texto simples de forma rápida e fácil.

Todo arquivo de documentação no MkDocs é um arquivo `.md` (por exemplo, `introducao.md`, `instalacao.md`).

---

### Títulos e Hierarquia

Títulos são cruciais para organizar seu conteúdo e torná-lo legível. No Markdown, você usa o sinal de cerquilha (`#`) para definir títulos. Quanto mais cerquilhas, menor o nível do título.

```markdown
# Título Principal (H1)

## Seção Principal (H2)

### Subseção (H3)

#### Detalhe (H4)

##### Mais Detalhe (H5)

###### Seis (H6)
```
---
Exemplos:

# Título Principal (H1)

## Seção Principal (H2)

### Subseção (H3)

#### Detalhe (H4)

##### Mais Detalhe (H5)

###### Seis (H6)
---

### **Parágrafos e Quebras de Linha**

Para criar um novo parágrafo, basta deixar uma linha em branco entre os blocos de texto.

```
Primeiro paragrafo da documentacao.

Segundo paragrafo. # Note a linha em branco entre eles.
```

Para uma quebra de linha sem iniciar um novo parágrafo, você pode adicionar dois espaços no final da linha anterior e então pressionar Enter.

```
Primeira linha
Segunda linha  # mas ainda faz parte do mesmo paragrafo
```

### **Formatação de Texto**
O Markdown oferece diversas opções para formatar seu texto:

* **Negrito** Use dois asteriscos ou dois underscores antes e depois do texto.  
```markdow
 **Texto em negrito** ou __Texto em negrito__
```

* *Italico* Use um asteriscos ou um underscores antes e depois do texto.  
```markdow
 *Texto em italico* ou _Texto em italico_
```

* ***Negrito e Itálico*** Combine os caracteres (três asteriscos ou três underscores).  
```markdow
 ***Texto em italico*** ou ___Texto em italico___
```

* **Monospace** (para linha de código): Use um único acento grave (backtick) antes e depois do texto. Ideal para comandos, nomes de variáveis ou trechos curtos de código.

Exemplo: Para instalar, use o comando `pip install mkdocs`
``` markdow
Para instalar, use o comando `pip install mkdocs`
```	

### Listas

#### Listas Não Ordenadas

Use asterisco (*), hífen (-) ou sinal de adição (+) para criar listas não ordenadas.

```
* Item 1
* Item 2
    * Subitem 2.1
    * Subitem 2.2
        * Sub-subitem 2.2.1
- Item 3
+ Item 4
```
Exemplo:

* Item 1
* Item 2
    * Subitem 2.1
    * Subitem 2.2
        * Sub-subitem 2.2.1
- Item 3
+ Item 4

#### Listas Ordenadas
Use números seguidos de um ponto. O Markdown automaticamente ajusta a numeração.
```
1. Primeiro item
2. Segundo item
   1. Subitem A
   2. Subitem B
3. Terceiro item
```

Exemplo:

1. Primeiro item
2. Segundo item
    1. Subitem A
    2. Subitem B
3. Terceiro item


### Links

Links são fundamentais para navegar entre páginas e referenciar recursos externos.

####Links Internos (entre páginas da documentação)
Para linkar para outras páginas dentro da sua documentação, use o caminho relativo do arquivo Markdown.  
```markdow
[Ir para a Introdução](introducao.md) # Entre chaves [] fica o titulo 
[Ver mais detalhes sobre a Instalação](instalacao/index.md) # Entre parênteses () fica o caminho
```
#### Links Externos
Para links de websites externos, inclua o protocolo (http:// ou https://).  
```markdow
[Visitar o site do MkDocs](https://www.mkdocs.org/)
```
Exemplo: [Visitar o site do MkDocs](https://www.mkdocs.org/) 

###Inclusão de Imagens
Para incluir imagens, a sintaxe é similar à de links, mas com um ponto de exclamação (!) no início.

```
![Texto da Imagem](caminho/para/minha/imagem.png)
```

* **Texto da imagem:** Descrição da imagem, importante para acessibilidade e caso a imagem não carregue.
* **Caminho da Imagem:** Pode ser um caminho relativo dentro da sua pasta docs ou uma URL externa.

###Blocos de Código (Code Blocks)
Para apresentar blocos de código com destaque e formatação adequada, use três acentos graves
(backticks) antes e depois do bloco, e opcionalmente, o nome da linguagem para melhor destaque.

```markdow
 ```bash
 # Este é um comando de exemplo
 mkdocs build
 pip install mkdocs-material

 ```
```
* Saida
```bash
# Este é um comando de exemplo
mkdocs build
pip install mkdocs-material
```

---

### Citações (Blockquotes)

Para citar um texto, use o sinal de maior que (`>`).

```markdow
> "Exemplo de texto."
> - Autor do texto
```
``` 
> "Texto de exemplo ou citação."
> - Autor
```

###Tabelas
Tabelas são criadas usando hífens (-) para separar o cabeçalho e barras verticais ( | ) para separar as colunas.

| Cabeçalho 1 | Cabeçalho 2 | Cabeçalho 3 |
|-------------|-------------|-------------|
| Conteúdo 1A | Conteúdo 2A | Conteúdo 3A |
| Conteúdo 1B | Conteúdo 2B | Conteúdo 3B |

* Exemplo
```markdow
| Cabeçalho 1 | Cabeçalho 2 | Cabeçalho 3 |
|-------------|-------------|-------------|
| Conteúdo 1A | Conteúdo 2A | Conteúdo 3A |
| Conteúdo 1B | Conteúdo 2B | Conteúdo 3B |
```

Você pode alinhar o conteúdo das colunas adicionando dois pontos (:) nos hífens de separação:

| Alinhado à Esquerda | Alinhado ao Centro | Alinhado à Direita |
|:--------------------|:------------------:|-------------------:|
| Item A              | Item B             | Item C             |
| Outro Item          | Mais Centralizado  | E à Direita        |

* Exemplo:
```markdow
| Alinhado à Esquerda | Alinhado ao Centro | Alinhado à Direita |
|:--------------------|:------------------:|-------------------:|
| Item A              | Item B             | Item C             |
| Outro Item          | Mais Centralizado  | E à Direita        |
```

###Linhas Horizontais
Para criar uma linha horizontal (separador visual), use três ou mais hífens (-), asteriscos (*) ou underscores (_) em uma linha separada.

---

***

___


```
---
___

***
```

