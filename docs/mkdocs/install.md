# Guia de Instalação do MkDocs

Este guia detalha os passos necessários para instalar o MkDocs em seu sistema. É um processo simples e rápido, que permitirá que você comece a criar sua documentação em pouco tempo.

---

## 1. Pré-requisitos

Antes de instalar o MkDocs, certifique-se de que você tem os seguintes softwares instalados em seu computador:

* **Python:** O MkDocs é construído com Python, então você precisará ter o Python 3.8 ou superior.
* **pip:** É o gerenciador de pacotes do Python e geralmente vem junto com a instalação do Python. Usaremos o `pip` para instalar o MkDocs.

### Como verificar se estão instalados:

Abra seu terminal ou prompt de comando e execute os seguintes comandos:  

```
bash python --version  
bash pip  --version    
```
Caso estejam instalados voce deve ver `Python 3.12.3 ` e ` pip 23.2.1 from dir/... ` , ou a versao que estiver instalada no seu sistema. 


## 2. Instalação do MkDocs
Agora Com o Python e o `pip` configurados
Execute o seguinte comando no seu terminal:  
`pip install mkdocs`  

Para verificar se foi instalado corretamente execute:
`mkdocs --version`  
Você deverá ver a versão do MkDocs instalada ex: `mkdocs, version 1.4.2 from dir/...` 

* Instalação de Temas Adicionais (Opcional)  
Para ter uma melhor experiencia visual é recomendado a instalação dos tema **Material for Mkdocs** 
`pip install mkdocs-material `


Caso esteja tudo ok , siga para as instruções de configuração aqui: [Configurando Mkdocs.](configurations.md) 
