# Listar branches
git branch

# Ver branch atualm com mais precisão
git branch --show-current

# Criar uma branch
git branch <nome_da_branch>

# Setar uma branch como atual
git checkout <nome_da_branch>
# ou 
git switch <nome_da_branch>

# Deletar uma branch
git branch -d <nome_da_branch>

# Juntar commits de uma branch com uma outra branch, ex:
# Temos duas branches: master e bug-fixes, imagine que a branch bug-fixes imagine que a branch bug-fixes esteja setada, quero que dê um merge com a branch master

git checkout master
git merge bug-fixes
git log --oneline

# -------------------------------------------------------

# Mandar uma branch criada no repositório local git para o repositório remoto(github)

# Vamos primeiro criar uma branch
git branch branch-exemplo

# Vamos manda-la para o nosso repositório remoto
git push -u origin branch-exemplo

# ----------------------------------------------------------

# Remover uma branch do repositório remoto (Github)
git push -d origin branch-exemplo

# Remover uma branch do repostório local GIT
git branch -d branch-exemplo

# Remover tanto do remoto tanto do local
git push -d origin branch-exemplo && git branch -d branch-exemplo
