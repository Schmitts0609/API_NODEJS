# Criando rotas

* Abra o Git Bash
## Baixar o arquivo do github:
* Cole o seguinte comando:
```
git clone COLAR_URL
```
## Entrar na pasta do arquivo:
* Para entrar na pasta do arquivo, cole o comando a seguir:
```
cd NOME_DO_ARQUIVO
```
## Reinstalar os pacotes da aplicação
* Este comando irá recriar a pasta node_modules no projeto:
```
npm i
```
## Criar pasta routes dentro da src:
* Execute o seguinte comando para criar a pasta routes:
```
mkdir src/routes
```
## Criar arquivos dentro da pasta routes:
* Crie o arquivo rotas.js dentro da routes:
```
touch src/routes/rotas.js
```
## Abrir o VSCode:
```
code .
```
## Abrir o arquivo rotas.js:
* Escreva o seguinte código:
```
// Importar o modulo de Router do express
const { Router } = require('express');

// Instanciar o Router na variável router
const router = Router();

router.get('/listar', (request, response) => {
    response.send('Método GET: listar informações');
});
router.post('/cadastrar', (request, response) => {
    response.send('Método POST: salvar informações');
});
router.put('/user/:id', (request, response) => {
    response.send('Método PUT: atualizar informações');
});
router.delete('/user/:id', (request, response) => {
    response.send('Método DELETE: remover informações');
});

module.exports = router;
```
## Abrir o arquivo app.js
* Digite os códigos:
```
const router = require('./routes/rotas');
```
```
app.use('/api', router);
```
## Atualizar o github com os arquivos modificados:
```
git add .
```
```
git commit -m 'rotas do projeto'
```
```
git push
```
## Excluir os arquivos do computador:
```
cd ..
```
```
rm -rf NOME_DO_ARQUIVO
```