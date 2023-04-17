# Listar todos os commits que tenham um nome de autor especificado
git log --author="Weslley"

# shotlog -> Mostra os autores dos commits, quantos commits fizeram e as mesnagem de cadas commit
git shortlog

# Obtendo o que foi adicionado, ou o que foi modificado em um commit através do seu id
git show <ID_COMMIT>

# Antes de dar um commit, use o comando a seguir para dar uma última visualizada na modifição

git diff

# -----------------------------------------------------------------
# VOLTAR O COMMIT FEITO
# -----------------------------------------------------------------

# Voltando um commit feito, supondo que tu fez um commit sem querer(por engano), então use o comando a seguir:

# --soft  ->  vai voltar para um commit, e matar o commit feito, mas os arquivos vão estar no staging area

# --mixed ->  vai voltar para um commit, e matar o commit feito, mas os arquivos vão estar antes staging area, vão estar por exemplo: modified ou untracked

# --hard  ->  vai voltar para um commit, e matar o commit feito, e matar todos os arquivos modificados, ou adicionados, ou removidos no commit.
.
# OBS: COLOCQUE O ID DO COMMIT ANTERIOR CASO QUERO SE DESFAZER DE UM OU MAIS COMMITS DEPOIS DO COMMIT ESCOLHIDO, CASO QUEIRA MODIFICAR COM SEGURANÇA, ALTERE UM COMMIT NO REPOSITÓRIO LOCAL ANTES DE MANDAR PARA O REMOTO

git reset --soft  <ID_COMMIT_ANTERIOR_AO_QUE_QUER_MUDAR>
git reset --mixed <ID_COMMIT_ANTERIOR_AO_QUE_QUER_MUDAR>
git reset --hard  <ID_COMMIT_ANTERIOR_AO_QUE_QUER_MUDAR>

# -----------------------------------------------------------------

# REMOVENDO UM GIT REMOTE ORIGIN (Vamos usar isto quando formos clonar e der errado, ai resstamos o caminho para o repositorio remoto)

git remote remove origin