# O comando 'git log' no dá o histórico dos nossos commits, com ele podemos voltar atrás em nosso commits por exemplo.

git log 

# Para ver o que um commit modificou basta usar o seguinte comando

git show id_commit

# Podemos adicionar ao staging area e commitar logo em seguida, com o comando 'git commit -am "mensagem do commit"'
# OBS: Este comando abaixo não irá funcionar para arquivos que estajam 'untracked', somente os arquivos que ja foram commitados.

git commit -am "Novo commit" 

# Podemos remover um arquivo do nosso repositório local (após feito o commit) e de nosso diretório do projeto, 
# Remove tanto do diretorio do projeto, tanto o repositório local do projeto git
# Este comando só irá funcionar após o arquivo ser commitado.
# OBS: Este comando não remove definitivamente um ficheiro, ainda podemos recupera-lo

git rm teste3.txt 

# Para remover o GIT de um projeto basta remover o diretório '.git'

# Usando o gitignore -> Para impedir que arquivos ou diretórios com arquivos seja commitados
# crie um arquivo .gitignore para impedir que o git envie arquivos/diretorios para o seu repositório local

# Mostrando o 'git log' em uma só linha para cada commit

git log --oneline