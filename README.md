# Carfinder - API

## URL do Projeto:
[Clique aqui](https://carfinder-api.herokuapp.com/)

## Para acessar o swagger:
[Clique aqui](https://carfinder-api.herokuapp.com/swagger/)

## Collections Insomnia:
[Clique aqui](Insomnia_2022-07-04.yaml)


###Publicando na Azure
------------------------------------------

Passo 1 Criar um fork do projeto para domínio do mesmo, uso.  <br>
Passo 2 Provisionar recursos dentro da Azure (App Services)  <br>
    - Devemos informar, resource group, nome da aplicação (o nome deve ser único), informar run time, informar sistema operacional selecionar o tamanho / configuração do hardware alocado.
Passo 3 abrir o repositório com o projeto par edição do mesmo.   <br>
Passo 4 devemos criar as pastas para criar nossa pipeline: diretórios (.github/workflows) arquivo de pipeline (prod.yml)   <br>


### Pipeline template:

```
name: Pipeline CI/CD - Prod

on:
  push:
    branches:
      - main
  workflow_dispatch:


jobs:
  build-and-deploy
    name: iniciando build e deploy
    runs-on: ubuntu-latest
    enviromments: production
```






### Projeto exclusivo Icarros <> GamaAcademy

### Professor Douglas Morais
#### Desenvolvido com NodeJS | GamaAcademy