
 #  Inserir nota de aula Módulo 3
 
 
**O ideal é que você não trabalhe na branch master que é criada no seu primeiro commit pelo Git, e busque usar a master para fazer push com o seu repositório remoto e seu código em desenvolvimento, coloque em uma branch, leve apenas códigos estáveis para o master**

 **Branchs - são separações de código, com elas , é possível que várias pessoas atuem em um mesmo projeto independente**
 
 **Digitando git branch sabemos quais branches temos no nosso repositório:**
 - git branch
 
 **Para criar uma nova branch é bem simples: git branch <nome da branch> então seria:**
 - git branch development
 
**Mudar de branch**
 
 git checkout [NOME BRANCH]
 
 **saber em qual branch estamos**
 git status
 
 ## Fazendo merge
 **Vamos para o local que queremos que as alterações sejam aplicadas, ou seja, a master**
 
 Git checkout master(Para garantir que você está na master, verifique git branch)
 
 - Agora vamos fazer o merge
 
 git merge [o branch que quero usar]
 **Estamos dizendo: me traga todas as modificações da branch development para master. Se tiver algum conflito, é agora que vamos saber.**
