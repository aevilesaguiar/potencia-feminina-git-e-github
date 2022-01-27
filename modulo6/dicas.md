1. Você sabe a diferença entre git e GitHub?
Git é o software de controle de versão, GitHub é uma plataforma para hospedar projetos que usam git. Fora o GitHub existem outras soluções como BitBucket e GitLab, e por ser open source você pode ter seu próprio servidor de git.

2. Como saber o que você fez?
git reflog

Esse comando fornecerá um histórico completo do que você fez.

3. Como adicionar mais algum arquivo depois de ter dado commit?
1) git add
2) git commit –amend

O amend irá modificar o commit anterior, então você pode utilizá-lo para remover arquivos do commit, mudar a mensagem, trocar autor, ou seja, fazer o que quiser!

4. Criei vários commit, mas não quero mais, e também não quero perder as mudanças feitas:
git reset –soft

As mudanças estarão staged, prontas para serem commitadas novamente.


5. Como apagar tudo (commits e mudanças) que fiz e deixar minha branch igual a um commit específico ou branch?
git reset –hard

Para deixar igual a uma branch remota, o comando é: git reset –hard origin/branch

6. Como commitar só uma parte das mudanças sendo que mexi em vários arquivos?
git add -p

Você irá ver parte por parte do que modificou e uma pergunta sobre o que deseja colocar em stage

7. Como ver o diff inteiro de código do que foi feito nos últimos commits?
git log -p

8. Como não subir arquivos indesejados em um projeto novo?
Basta configurar o arquivo .gitignore. Será mais fácil se você fizer isso no início do projeto ao invés de ter que remover depois.

Vou deixar abaixo uma lista de templates para você copiar:

github/gitignore – A collection of useful .gitignore templates. Contribute to github/gitignore development by creating an account on GitHub.

9. Como fechar uma issue automaticamente?
No GitHub, escreva na mensagem do commit “closed”, “closes”, “close”, “fixed” ou “fixes” seguido de hashtag + número da issue (exemplo: “Fixes #1234”) , a issue será fechada imediatamente.

10. Se você usa o VS Code, recomendo fortemente o plugin Git Lens.
Ele irá te mostrar de forma visual todo o histórico de commits do arquivo, quem fez e quando foi feito, muito útil:

GitLens — Git supercharged – Visual Studio Marketplace

11. Como acompanhar o fork de um projeto?
git remote add <https://url-do-fork.git>

Para ver todos os remotes do repo que você tem localmente:

git remote -v

Para usar, é só trocar origin pelo nome que você deu ao remote:

git pull , git checkout nome-fork/branch…

12. Como não correr o risco de perder o que já foi feito mesmo que você ainda não tenha concluído?
Quanto mais detalhada for a descrição do commit, melhor será futuramente, principalmente se seu código não for muito comentado.

13. Escreva mensagens de commit concisas e específicas.
Basta você commitar e adicionar na mensagem “WIP” antes, que significa Work in Progress.

Quando estiver tudo pronto é só dar commit –amend e tirar o WIP da mensagem.

14. Quanto mais commits melhor.
A função funcionou? commita. O teste passou? commita.

Essa tática vai te ajudar bastante no futuro caso precise desfazer algo, buscar bugs ou reaproveitar seu código.

Mesmo que ainda não esteja 100%, commita com “WIP” na frente.

15. Mais sobre WIP: essa dica irá servir quando você estiver numa branch separada.
Se tiver trabalhando com alguém na mesma branch, é bom avisar para não correr o risco de mandar código quebrado pro seu parceiro.

Evite mandar WIP pra master, já que devemos sempre evitar modificar o passado dessa branch

16. Como fazer alguma modificação em um commit do passado que não seja o último?
Por exemplo para tirar um commit WIP, usamos o git rebase -i, que é o rebase interativo.

17. Criou uma branch com o nome errado e só percebeu depois, na hora de dar push?
Calma, não é o fim:

git branch -m nome-velho nome-novo

18. Tem dificuldade com vim ou outro editor de linha de comando?
Você pode muito bem trocar o editor padrão que o git usa para escrever as mensagens de commit ou resolver conflitos:

git config –global core.editor “seu-editor”

19. É entediante ter de adicionar arquivo por arquivo?
Ao invés de dar git add . e vez ou outra subir o que não deve, use git add -u que ele vai adicionar só os arquivos que já foram trackeados pelo git. Ou seja, nunca use git add.

20. Use git stash pra guardar temporariamente os arquivos modificados que ainda não foram commitados.
Útil quando precisa trocar de branch, por ex: testar o código sem suas mudanças, ou testar em outra branch. Pra “pegar” as mudanças de volta git stash pop.