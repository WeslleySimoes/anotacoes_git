# Listar todos os commits que tenham um nome de autor especificado
git log --author="Weslley"

# shotlog -> Mostra os autores dos commits, quantos commits fizeram e as mesnagem de cadas commit
git shortlog

# Obtendo o que foi adicionado, ou o que foi modificado em um commit através do seu id
git show <ID_COMMIT>

# Antes de dar um commit, use o comando a seguir para dar uma última visualizada na modifição

git diff