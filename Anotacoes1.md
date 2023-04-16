#--------------------
#  Usando o git
#--------------------

# para ver a versão do git
git --version
git -v 

#--------------------------
# CONFIGURAÇÕES INICIAIS APÓS O DOWNLOAD DO GIT (Configuradas uma única vez, mas podendo com os mesmos comandos alterá-las)
#--------------------------

# Definindo o nome do utilizador da git
git config --global user.name "Weslley Simões" 

# Definindo o nome do utilizador da git
git config --global user.email "weslley_silvas@hotmail.com" 

# Definindo o nome padrão para a branch prinicpal
git config --global init.defaultBranch nome_novo_da_branch

# Podemos ver as nossas variaveis globais definidas
git config --global --list 

#--------------------------
# CRIANDO O NOSSO PRIMEIRO REPOSITÓRIO LOCAL
#--------------------------

# Iniciando um repositório local (que por padrão é vazio, porque ainda não comitamos os arquivos)
git init

# Mostra um conjunto de informações
git status 

# VAMOS ADICIONAR O FICHEIRO 'INDEX.HTML' PARA SER CONTROLADO PELO NOSSO VERSIONAMENTO
git add index.html

# Para voltar a ação anterior de 'git add' e remover o arquivo 'index.php' do staging area
git rm --cached index.html

# Commitando um arquivo (Definindo ele como arquivo final funcional em nosso diretório local)
git add -m 'Primeiro commit'

# Depois de ter dado o commit, podemos usado o 'git status' para verificar se há algum arquivo que precisa ser commitado
git status

# Para ter certeza que houve um commit podemos usar o comando 'git log', que o histórico de commits
git log

# Após adiciona mais um arquivo no staging area, e querer retorna-lo para fora do controle do git,
# use o comando 'git restore --staged arquivo.extensao' ou 'git rm --cached arquivo.extensao'
git restore --staged script.js

# Mostrando o git status resumido -s de short
git status -s 

# Se adiconarmos 3 arquivos e quisermos mover esses 3 arquivos de uma só vez para a staging area, usando o comando 'git add .'

git add .

# Se quisermos remover esses 3 arquivos do staging area, usando o comando 'git restore --staged .'

git restore --staged .

