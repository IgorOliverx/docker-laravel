# Configurando um Ambiente de Desenvolvimento Laravel com DOCKER

## Índice
- [Windows](#windows)
- [Linux](#linux)

## Windows

### 1. Clonando o Repositório no WSL
Primeiro, certifique-se de ter o WSL (Windows Subsystem for Linux) configurado no seu sistema. Se você ainda não o configurou, siga o [guia oficial de instalação do WSL](https://docs.microsoft.com/pt-br/windows/wsl/install) para prepará-lo.

Depois que o WSL estiver configurado, abra um terminal WSL e navegue até o diretório onde deseja clonar o repositório do seu projeto Laravel. Execute o comando abaixo para clonar o repositório:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

Substitua `https://github.com/seu-usuario/seu-repositorio.git` pela URL do repositório que deseja clonar.

### 2. Rodando o Docker Compose
Após clonar o repositório, navegue até o diretório do projeto:

```bash
cd seu-repositorio
```

Agora, execute o seguinte comando para construir e iniciar os contêineres Docker:

```bash
docker-compose up -d --build
```

Esse comando irá construir os contêineres definidos no arquivo `docker-compose.yml` e iniciá-los em segundo plano. A opção `--build` garante que as imagens Docker sejam construídas novamente, o que é útil se você fez alterações nos Dockerfiles.

---

## Linux

### 1. Clonando o Repositório
Abra um terminal e navegue até o diretório onde deseja clonar o repositório do seu projeto Laravel. Execute o comando abaixo para clonar o repositório:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

Substitua `https://github.com/seu-usuario/seu-repositorio.git` pela URL do repositório que deseja clonar.

### 2. Rodando o Docker Compose
Após clonar o repositório, navegue até o diretório do projeto:

```bash
cd seu-repositorio
```

Agora, execute o seguinte comando para construir e iniciar os contêineres Docker:

```bash
docker-compose up -d --build
```

Esse comando irá construir os contêineres definidos no arquivo `docker-compose.yml` e iniciá-los em segundo plano. A opção `--build` garante que as imagens Docker sejam construídas novamente, o que é útil se você fez alterações nos Dockerfiles.

---

Com esses passos, você terá um ambiente de desenvolvimento Laravel configurado usando Docker tanto no Windows quanto no Linux. Se precisar de mais ajuda, consulte a documentação oficial do Docker e Laravel.
