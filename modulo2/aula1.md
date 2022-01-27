## Notas de aula módulo2

- Primeiro é necessário instalar o git na máquina:https://git-scm.com/downloads

## Para criarmos um repositório será necessário criar uma pasta, após isso abra ela e execute o comando “git init“.

**Adicionando o repositório ao seu projeto**

- Com o cadastro no Github feito, e com o seu repositório devidamente criado, agora vamos adicioná-lo ao projeto local na sua máquina.
Para começar, acesso o diretório do seu projeto.

cd /Users/gbgelado/projeto

- Inicie o Git e adicione o repositório.
git init

- git remote add origin https://github.com/gbgelado/meu-primeiro-repositorio.git

**Agora é a hora de adicionar os arquivos, "commitar" e "pushar"**
git add .
git commit -m "meu primeiro commit"
git push -u origin master

**Para publicar seu projeto no repositório remoto, é necessário estar autenticado. O Github vai pedir seu usuário e senha sempre que você der um git push e isso não é muito legal por que existe uma maneira muito mais simples.**

$ git push origin master
Username for 'https://github.com':
SSH Key

- Na documentação do Github há um passo-a-passo muito simples de como criar e adicionar seu ssh key na sua conta do Github.
Após concluído esse processo, precisamos o repositório remoto em nosso projeto.

**Vamos remover o repositório antigo:**

git remote remove origin

**E adicionar o novo:**
git remote add origin git@github.com:gbgelado/meu-primeiro-repositorio.git

**Dar um push**
$ git push origin master
