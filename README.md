# Página do Núcleo de (ex-)bolsistas do Brasil no exterior

Este repositório contém o código fonte da página <https://exbolsistas.org>.

Esta página é contruida usando [MkDocs](https://www.mkdocs.org/) e o tema [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/). 

## Como fazer parte do Núcleo

Veja <https://exbolsistas.org/faça-parte/> ou [docs/faça-parte.md](docs/faça-parte.md).

## Como contribuir com o Núcleo

Ainda não temos uma documentação sobre como contribuir com o Núcleo, e ainda não definimos uma licença para o conteúdo desse repositório, mas sinta-se a vontade para enviar sugestões através de GitHub issues e Pull Requests.

## Como servir a página localmente

Para servir a página localmente (i.e. no seu computador), é necessário um ambiente capaz de rodar containers com [Docker Compose] (e.g., com [Docker Desktop] ou [Podman Desktop]), ou um ambiente capaz de rodar scripts em Python (testado com Python 3).

[Docker Compose]: https://docs.docker.com/compose/
[Docker Desktop]: https://www.docker.com/products/docker-desktop/
[Podman Desktop]: https://podman-desktop.io/

Abaixo seguem as instruções para ambas a opções de ambiente de desenvolvimento.

### Ambiente com containers

Após clonar esse repositório, use o comando `docker compose up` ou `docker-compose up`.

A página estará disponível no endereço <http://localhost:8000/>.

### Ambiente com Python nativo

Para evitar conflito com outros ambientes de desenvolvimento locais, as intruções abaixo fazem uso de ambientes virtuais (<https://docs.python.org/3/library/venv.html>).

Após clonar esse repositório, use os seguintes comandos em um terminal/linha de comando na raiz do repositório:

1. `python3 -m venv .devenv`
2. Em um prompt do Windows (Command Prompt, cmd.exe): `.devenv\Scripts\activate.bat`  
    Verifique <https://docs.python.org/3/library/venv.html#how-venvs-work> para instruções para outros terminais, linhas de comando e sistemas 
<!-- A versão usada aqui deve ser a mesma que a versão usada em .github/workflows/ci.yml -->
3. `pip3 install mkdocs-material==9.5.33`

Depois de seguir as instruções acima, você pode servir o site com o comando `mkdocs serve`.

A página estará disponível no endereço <http://localhost:8000/>.

Se você sair da linha de comando, será necessário ativar novamente o ambiente virtual, com o comando da instrução número 2.

**Nota:** O nome de ambiente `.devenv` foi escolhido arbitrariamente.

## Contato e Suporte

Veja <https://exbolsistas.org/SUPPORT/>, ou [docs/SUPPORT.md](docs/SUPPORT.md).