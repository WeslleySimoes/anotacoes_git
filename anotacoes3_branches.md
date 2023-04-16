# Obtendo o nome da branch atual
git branch --show-current

# Listando a branches disponíveis
git branch

# Criando uma branch chamada bug-fixes
git branch bug-fixes

# Mudando o branch atual para um outro
git checkout <nome-do-branch>
ou
git switch <nome-do-branch>

# Criando uma branch e setando ela como atual
git checkout -b <nome-do-branch>

# Obtendo os commits da branch bug-fixes para a master, ou seja, juntando os que estão na branch bug-fixes para master
# OBS: o GIT irá observar se há conflitos entre os commits da duas branches, e cabe ao programador escolher qual commit irá de consolidado
git checkout master
git merge bug-fixes

# Apagando uma branch
git branch -d <nome-da-branch>

# #########################################################

# Pega o código do commit que está em amarelo
git log --oneline

# Navegando entre commits de uma branch atual
# Este comando abaixo, resultara como se fosse uma branch nova, obtendo os commits até o commit escolhido, para reverter o comando abaixo basta digitar 'git checkout <NOME_BRANCH>', neste caso ele irá voltar para ulítmo commit da branch principal
git checkout <ID_COMMIT>

# Caso queria acessar um commit mas continuar na branch atual, basta usar o comando acima com o ponto no final:
# Para voltar ao último commit da branch basta usar o mesmo comando, mas com o id do último commit
git checkout <ID_COMMIT> .

# OS COMANDOS DE NAVEGAÇÃO É BASTANTE UTILIZADOS PARA ANALISAR O CÓDIGO QUE FOI FEITO EM UM COMMIT ANTERIOR.