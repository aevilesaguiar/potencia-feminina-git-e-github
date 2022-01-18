# Notas de aula referentes ao módulo 1 do curso git e github da potencia feminina

### Nota 1 - criando o repositório local e remoto
### Nota 2 - nesta aula estamos aprendendo os comandos 
**git commit - conjunto de alterações do código**
**git status-verifica o status do arquivo**

### Nota 3 - nesta aula estamos aprendendo os comandos 
**git add - esse comando realiza a inclusão ou modificação do arquivo no diretório local, preparando para ele ser entregue ao servidor**

### git status
 **verificar o status dos arquivos e pastas dentro do nosso repositório**

 ### git add [caminho do arquivo]

 **adicionar um arquivo em específico**

### Revendo

#### Comandos Git básicos
**1. git config**
Quando você está utilizando o Git pela primeira vez ou com uma instalação nova, em um projeto colaborativo, esse comando é fundamental para configurar sua identidade de usuário, inserindo informações como nome e email que serão empregadas em cada commit.

Exemplo:

$ git config –global user.name “Seu nome”

$ git config –global user.email “Seu email”

**2. git init**
Esse é o comando que você irá utilizar para criar um novo projeto de git. O comando irá criar um repositório novo em branco e, a partir daí, será possível armazenar seu código fonte, alterar, salvaguardar alterações etc.

Exemplo:

$ git init

Se você já possui um repositório anterior ou deseja criar um repositório com um nome em específico, você pode passar o nome como parâmetro do comando:

$ git init <O nome do seu repositório>

**3. git clone**
Esse comando Git cria uma cópia exata de um repositório já existente.

Então… quando usar git init e quando usar git clone? O git clone é mais avançado, uma vez que ele mesmo executa um comando git init internamente. Além disso, ele verifica todo o conteúdo do projeto.

Exemplo:

git clone <URL do seu projeto>




