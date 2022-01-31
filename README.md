# Notas de aula referente ao curso git e github da potencia feminina e WomakersCode

## Modulo 1 
[Conceitos Iniciais](https://github.com/aevilesaguiar/potencia-feminina-git-e-github/blob/main/modulo1/aula1-notas-de-aula.md)
<br>
## Modulo 2 
[ Criando seu primeiro repositório e apresendendo comandos mais utilizados](https://github.com/aevilesaguiar/potencia-feminina-git-e-github/blob/main/modulo2/aula1.md)
<br>
## Módulo 3
[ Trabalhando com branchs](https://github.com/aevilesaguiar/potencia-feminina-git-e-github/blob/main/modulo-3/criando-uma-nova-branch.md)
<br>
## Módulo 4
[  Colaborando com projetos de outras pessoas](https://github.com/aevilesaguiar/potencia-feminina-git-e-github/blob/main/modulo4/aula1.md)
<br>
## Módulo 5 
[Conhecendo o github project](https://github.com/aevilesaguiar/potencia-feminina-git-e-github/blob/main/modulo5/aula.md)
<br>
## Módulo 6 
[Revisão e Dicas](https://github.com/aevilesaguiar/potencia-feminina-git-e-github/blob/main/modulo6/dicas.md)


## O fork eu fiz 
https://github.com/aevilesaguiar/potencia-feminina-git-e-github-1
<br>
https://github.com/aevilesaguiar/potencia-feminina-git-e-github-1/blob/master/pull%20request%20alunas.md



## Comentários Mentoria

- Rollback desfazer uma mudança que vc fez

- Padrões de rollback 
- usando o comando revert que cria um novo commit que foi feito no commit anterior. Cria uma nova alteração em coma do que já foi feito. 
- Padrões de mensagem de commit - depende de contextos. Commit em Ingles, mensagem de commit não passar de 80 caracteres. Separar o commit por unidade atomica, ou seja ex: fix type, se baseio no commit para fazer determinadas coisas. No corpo do commit eu incluo o motivo de fazê-lo. Sempre tento atrelar a uma issue.
- Extensão do  git para facilitar os comitts  :commitizen
- git-stash - Esconda as alterações em um diretório de trabalho sujo.Use git stashquando quiser gravar o estado atual do diretório de trabalho e o índice, mas quiser voltar para um diretório de trabalho limpo. O comando salva suas modificações locais e reverte o diretório de trabalho para corresponder ao HEADcommit. As modificações guardadas por este comando podem ser listadas com git stash list, inspecionadas com git stash show, e restauradas (potencialmente em cima de um commit diferente) com git stash apply. Chamar git stashsem argumentos é equivalente a git stash push. Por padrão, um stash é listado como "WIP no nome da ramificação …​", mas você pode fornecer uma mensagem mais descritiva na linha de comando ao criar um. O último stash que você criou é armazenado em refs/stash; stashes mais antigos são encontrados no reflog desta referência e podem ser nomeados usando a sintaxe usual de reflog (por exemplo stash@{0}, é o stash criado mais recentemente, stash@{1}é o anterior, stash@{2.hours.ago} também é possível). Os stashes também podem ser referenciados especificando apenas o índice do stash (por exemplo, o inteiro né equivalente a stash@{n}.
- git-revert - Reverte alguns commits existentes
- git switch -c nova-branch - substituiu o git checkout
- o projeto principal é salvo no main, default, ou o nome da task
- git-flow são padrões , recomendações - https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow . Exemplo brach : feature - , bug - , 
- 
- https://gitfichas.com/ algumas fichas 

- git commit --amend  alterando o último commit 
- 
- 
## Referencias

https://potenciafeminina.myedools.com/enrollments/6612582/courses/48734

https://git-scm.com/doc

https://docs.github.com/pt/pages

https://cantinhobinario.com/2021/03/28/20-dicas-poderosas-de-git-e-github-para-organizar-sua-vida/

https://womakerscode.org/

https://www.atlassian.com/git/tutorials/rewriting-history

https://www.alura.com.br/artigos/git-os-novos-comandos-git-restore-e-git-switch?gclid=Cj0KCQiArt6PBhCoARIsAMF5wai5Bh2eMXxiFnB9Ew5vG7oYOfR7JMzGICZTSZ65AzHTFiC57tIjMcwaAg17EALw_wcB

https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

https://www.npmjs.com/package/commitizen



