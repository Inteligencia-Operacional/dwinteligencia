# DWInteligencia - DB

Projeto criado para versionar os schemas e tabelas do banco SQL Server DWINTELIGENCIA.

Ferramenta utilizada foi a versão free do dbdocs.io.
Maiores informações e documentação pode acessar: https://dbdocs.io/docs

---------------------

### Como instalar o dbdocs em seu local de trabalho

### Pré-requistio:
- NodeJS
- NPM

### Instalação
Execute o seguinte comando no terminal:
```
npm install -g dbdocs
```
Ou se você estiver usando yarn
```
yarn global add dbdocs
```
Observe que, em alguns casos, você precisa adicionar ao seu comando para poder instalar dbdocs globalmente.```sudo npm```
```
$ sudo npm install -g dbdocs
dbdocs install...
```

Execute o comando para verificar se ele já foi instalado e visualizar alguns comandos.dbdocs
```
$ dbdocs
dbdocs ======

VERSION
  dbdocs/0.6.2 win32-x64 node-v12.16.1

USAGE
  $ dbdocs [COMMAND]
  
COMMANDS
  build     build docs
  help      display help for dbdocs
  login     login to dbdocs
  logout    logout
  ls        list projects
  password  set password for your project or remove password
  remove    remove project
  token     generate or revoke your authentication token
  validate  validate docs content
```
### Faça login no dbdocs
Antes de gerar a visualização dbdocs, você precisa fazer login executando o seguinte comando (login via e-mail)
```
$ dbdocs login
? Choose a login method: Email
? Your email: <your email address>
✔ Request email authentication
? Please input OTP code sent to the email:
```
Ao digitar corretamente o código OTP no e-mail, você poderá acessar os dbdocs.

![image](https://github.com/Inteligencia-Operacional/dwinteligencia/assets/142241021/e3ed8a41-de9f-478b-b132-60cb869dbf6c)

### Build e Publish do projeto no dbdocs
Abra a pasta que contém o arquivo dbml no terminal e, em seguida, gere a exibição dbdocs pelo comando a seguir.
```
$ dbdocs build <path to your dbml file>/seu_arquivo.dbml
Pushing new database schema to project your_project...
Done. Visit: https://dbdocs.io/sua_conta/seu_projeto
```

Em nosso exemplo a URL do projeto que ele vai gerar vai ser: https://dbdocs.io/estatistica/DWInteligencia
