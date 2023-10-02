# Documentação segunda parte

* Clonar o repositório do github para a máquina:
```
git clone URL_REPOSITORIO
```

* Acessar a pasta:
```
cd nomeDaPasta
```

* Reinstalar os pacotes da aplicação:
```
npm i
```

* Criar arquivo .env na raiz do projeto:

Ctrl + O: Salvar

Enter: Confirmar

Ctrl + X: Fecha
```
nano .env
```

* Digitar no arquivo .env:
```
PORT = 3008
```

* Adicionar .env ao .gitignore:
```
nano .gitignore
```
```
.env
```

* Abrir o VSCode:
```
code .
```

Criar arquivo de exemplo para para as variáveis necessárias da aplicação:
```
nano .env.example
```
```
PORT = 
```

* Abrir o app.js e digitar:
```
const express = require('express');
```
```
const dotenv = require('dotenv').config();
```
```
const app = express();
```
```
app.set('port', process.env.PORT || 3333);
```
```
module.exports = app;
```

* Abrir o server.js e digitar:
```
const app = require('./app');
```
```
const port = app.get('port');
```
```
app.listen(port, () => {
    console.log(`Running on port ${ port }!`);
});
```

* Abrir o package.json e alterar "test" para o seguinte:
```
"start":"nodemon src/server.js"
```

* Executar o servidor:
```
npm run start
```

# Enviar para o github

* Verificar o status do git:

```
git status
```

* Adicionar arquivos ao versionamento:

```
git add .
```

* Salvar o projeto e escrever um comentario da alteração realizada:

```
git commit -m 'estrutura do projeto'
```

* Enviar os arquivos para o github:

```
git push -u origin main
```