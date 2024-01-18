criar o repositório no github

verificar se tem algum repositório remoto

git remote -v
(não vai aparecer nada pq nao tem )

colar o código do seu repositório
git remote add origin https://github.com/sarahaffonco/curso-git-e-github.git
git branch -M main
git push -u origin main

git remote -v (vai aparecer o repositório)

ex: PS C:\Users\sarah\git-e-github> git remote -v 
origin  https://github.com/sarahaffonco/curso-git-e-github.git (fetch)
origin  https://github.com/sarahaffonco/curso-git-e-github.git (push)

clonar o diretório
retornar a pasta raiz cd ..//
mkdir teste-clone para criar outro diretório
cd teste-clone (selecionar o diretório teste-clone)
copiar o cógido de clone do github
git clone https://github.com/sarahaffonco/curso-git-e-github.git

*para alterar a pasta que esta, sempre volta para pasta raiz e altera*
cd ..// 
cd "nome-da-pasta"

comando git status
**verifica se teve alteração da pasta dentro do repositório **

### adicionando arquivos para esteira de commit
git add . (adiciona todos os arquivos)
git add ("nome-especifico) (para adicionar arquivo específico)

### git commit 
registro dos comandos, tem codigo unico de uma alteraçao (utilizado para desfazer/refazer alteração)

git commit -m "nome"

### git push

**primeiro se faz o upstream - para configurar e alinhas informações com github

git push --set-upstream origin *main* ou *master* conforme configuração do seu github

♥ prontinho, tudo está no github ♥

no github as abas "main" se refere as branchs (próximas aulas )

para desfazer o commit 
Caso não tenha feito o commit ainda, utilize:

git reset <arquivo-ou-diretório>
Caso já tenha realizado um commit, utilize:

git rm --cached <arquivo>
git rm -r --cached <diretório>