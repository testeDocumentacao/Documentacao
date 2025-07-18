# Configurando repositório e publicando no GitHub Pages

Após criar sua documentação com o **MkDocs**, você pode publicá-la gratuitamente usando o **GitHub Pages**, que permite hospedar sites estáticos diretamente de um repositório GitHub.

## Pré-requisitos

- Conta no [GitHub](https://github.com/).
- Repositório criado para o seu projeto.
- Git instalado na máquina.
- Documentação configurada com MkDocs.

---
##Inicializando repositório local

Dentro do diretório do seu projeto, inicialize o Git e conecte ao repositório remoto:

```bash
git init
git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git
```
Adicione e envie o projeto inicial aós fazer as configurações iniciais do github em sua máquina local  
( nome de usuario , e-mail , senha e o token para enviar os dados )
```bash
git add .
git commit -m "Versão inicial da documentação com MkDocs"
git push -u origin main
```
##Construindo o site estático
Antes de publicar, é necessário gerar os arquivos estáticos do seu site:
```
# Este comando cria a pasta 'site/' com os arquivos finais
mkdocs build
```
## Publicando
O MkDocs facilita a publicação usando o comando:
`mkdocs gh-deploy`

Esse comando:

* Cria o build da documentação.
* Cria (ou atualiza) automaticamente o branch gh-pages no seu repositório.
* Publica os arquivos da pasta site/ no GitHub Pages.

E gera o site no caminho do seu repositorio: `https://Nome_De_Usuario.github.io/Pasta_Do_Projeto/`
