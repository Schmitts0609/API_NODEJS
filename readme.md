# Documentação

* ### Abrir o GitBash na área de trabalho
* ### Criar pasta utilizando o comando (make directory):

```
mkdir projetoBackend
```

* ### Entrar na pasta utilizando o comando (change directory):

```
cd projetoBackend
```

* ### Iniciar o gerenciador de pacotes Node:

```
npm init -y
```

* ### Instalar os pacotes utilizando o comando:

```
npm i express nodemon dotenv
```

* ### Abrir o VSCode do arquivo:

```
code .
```

* ### Criar o arquivo .gitignore utilizando o comando:

```
nano .gitignore
```

* ### Adicionar a pasta dos módulos dentro do .gitignore:

```
node_modules
```

* ### Depois disso, dar CTRL+O para salvar, Enter para confirmar e CTRL+X para deixar o espaço nano
* ### Criar a pasta de arquivos utilizando o comando (make directory):

```
mkdir src
```

* ### Criar o arquivo de configuração e execução da api dentro da pasta source:

```
touch src/app.js
```

* ### Criar o arquivo responsável por receber as configurações e rodar a api:

```
touch src/server.js
```

* ### Criar pasta para gerenciar as rotas da API:

```
mkdir src/routes
```

* ### Inicializar gerenciador de arquivo .git

```
git init
```

* ### Informar nome e email:

```
git config --global user.name 'primeiro-nome'
```

```
git config --global user.email 'seu-email'
```

* ### Verificar o status do git:

```
git status
```

* ### Adicionar arquivos ao versionamento:

```
git add .
```

* ### Salvar o projeto e escrever um comentario da alteração realizada:

```
git commit -m 'estrutura do projeto'
```

* ### Definir o branch para main:

```
git branch -M main
```

* ### Informar o repositório que queremos enviar o arquivo:

```
git remote add origin COLAR_URL
```

* ### Enviar os arquivos para o github:

```
git push -u origin main
```