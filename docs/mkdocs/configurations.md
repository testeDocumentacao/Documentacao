# Configurando o MkDocs

Este guia irá auxiliá-lo na configuração inicial do seu projeto MkDocs.

---

## 1. Criando um Novo Projeto MkDocs

Com o MkDocs já instalado, o próximo passo é criar o projeto de documentação.

* **Defina o local:** Navegue até o diretório onde deseja criar os arquivos base do MkDocs.
Exemplo: `bash cd Documentos/`

* **Crie o projeto:** Execute o comando `mkdocs new` seguido do nome desejado para o seu projeto.  
Exemplo: `bash mkdocs new meu-projeto-docs`. Isso criará uma nova pasta com o nome escolhido do projeto Ex: `meu-projeto-docs`, com a estrutura básica:

```
    meu-projeto-docs/
    ├── mkdocs.yml
    └── docs/
        └── index.md
```

* **Navegue até o diretório do projeto:**
    `bash cd meu-projeto-docs`

---

## 2. Visualizando sua Documentação

Para ver sua documentação em tempo real enquanto você a edita:

* **Inicie o servidor de desenvolvimento:** Dentro do diretório do seu projeto, execute:  
`bash mkdocs serve`, Você verá uma mensagem indicando o endereço local do servidor, como:
`INFO - [HH:MM:SS] Serving on http://127.0.0.1:8000/`

* **Especifique uma porta diferente (se necessário):** Caso a porta padrão (8000) esteja em uso, você pode indicar uma porta alternativa:
    ```bash
    mkdocs serve --dev-addr 0.0.0.0:8001
    ```
    Substitua `8001` pela porta desejada.

* **Acesse no navegador:** Abra seu navegador web e navegue para o endereço indicado (ex: `http://127.0.0.1:8000/` ou `http://127.0.0.1:8001/`).

Com esses passos, você terá sua primeira documentação MkDocs funcionando e pronta para ser editada!
