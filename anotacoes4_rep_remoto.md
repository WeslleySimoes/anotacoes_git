# Clonando um repositório para trabalhar localmente em nossa maquina e depois se quisermos sincronizarmos com o repositório remoto (Github por exemplo)

# Clonando via HTTPS, o 'git clone' irá neste caso criar uma pasta 'git_exemplo' com os arquivos

# OBS: ele irá pedir um atutenticação(login) para verificar se você tem diretiro de clonar o repositório

git clone https://github.com/WeslleySimoes/git_exemplo.git

# *************************************************************

# Conectando o nosso repositório local com o remoto e atualizando os arquivos(dados)
git push    

# Conectando a um branch especifico e enviado as alterações
git push origin <NOME_BRANCH>

# Sincronizando nossa branch criada no repositório local com o remoto

git push -u origin <NOME_BRANCH>

# Sincronizando nossa branch remota e trazendo alterações para o nosso repositório local
# OBS: Pode ocorrer de ter conflitos entre arquivos que possuem os mesmos códigos, cabe a você saber qual escolher
git pull