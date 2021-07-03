# git init = cria o repositório vázio dentro de um diretório, ou seja um outro local ou pasta

## untracked e tracked

# Untracked = são os arquivos ao qual ainda não se ha ciência deles

# TRacked = é o oposto de untracked e se divide em tres partes: Unmodified, modified e staged

# Unmodiefied é o arquivo que ainda não foi modificado

# Modified é o arquivo Unmodified que sofreu uma alteração este muda altomaticamente de unmodified para modified

#######################################################

# git status verifica o status de um arquivo no repositório

# o comando mv move um arquivo ou diretório para outro
## ex: mv arquivo.py ./diretório/...

# ao mover um arquivo para outra pasta dentro do repositório, o mesmo será considerado como deletado, então uma sugestão é utilizar o git add <com o nome do arquivo> <e o nome da pasta>, no final será colocado como renomeado em vez de excluído

# git rm <arquivo> remove o arquivo

# git restore <arquivo>, descarta as modificações feitas no working directory, ou seja restaura ao que era antes

# git restore --staged <nome do arquivo>, tirá o arquivo da area de staged

## Reescrevendo configurações do git
### git config --global --unset <a propriedade do git a ser alterado>

ex: git config --global --unset user.email
ex2: git config --global --unset core.editor

#### obs: fazer a alteração de email e usuario n~~ao afetara os arquivos comitados no git, mas pode apaercer de forma diferente no github

README são arquivos que contam as funcionalidades do sistema que foi desenvolvido


# adicionando a origem remota (o repositório do github) no git bash

depois de criado o resitório no github, basta abrir o git bash e digitar o seguinte comando

### git remote add origin <link do repositório>
ex: git remote add origin https://github.com/Milton-Luis/livro-receitas.git

origin é apenas um apelido para não ter que toda hora ficar digitando o endereço https o tempo inteiro, por convenção usamos origi

# listando o repositórios já cadastrados
### git remote -v: faz a listagem de repositórios cadastrados

# empurrando o git

### git push origin master
origin = apelido
master é a branch principal
