## Exemplos GitFlow ##

![img](https://github.com/nathan-oliveira/GitFlow/blob/main/GitFlow.PNG)
![img](https://github.com/nathan-oliveira/GitFlow/blob/main/GitFlow2.PNG)

## Comandos GitFlow ##

git flow init

##

git flow feature start criar_giropops

git flow feature publish criar_giropops

git flow feature finish criar_giropops

git flow feature pull criar_giropops

##

git flow release start 1.0

git flow release finish 1.0

##

git flow hotfix start my_hotfix

git flow hotfix finish my_hotfix

##

git config --add gitflow.multi-hotfix true

##

build:    alterações que afetam o sistema de build ou dependências externas

ci:       mudanças em arquivos e scripts de configuração de CI

chore:    outras mudanças que não modificam src ou arquivos de teste

docs:     alterações apenas na documentação

feat:     um novo recurso

fix:      uma correção de bug

perf:     uma mudança de código que melhora o desempenho

refactor: uma alteração de código que não corrige um bug nem adiciona um recurso

style:    alterações que não afetam a funcionalidade do código

test:     adicionar testes ausentes ou corrigir testes existentes

##

*** Eslint Fix ***

yarn lint --fix

*** Salvar arquivos modificamos em cache ***

git stash

*** Iniciar o GitFlow ***

git flow init -d

*** Criar o nome da feature, por exemplo ***

git flow feature start listagemPedidos

*** Voltar os arquivos modificamos que estava em cache ***

git stash pop

*** Git Add e Commit ***

git c "feat: "

*** Enviar as alteração para "git"***

git flow publish

*** FINALIZAR feature e enviar para DEVELOP ***

git flow finish --push  (ESQ :wq)

git flow feature finish --push

##

*** Criar release (Ambiente de homologação) ***

git flow release start v1.34.0

*** FINALIZAR release e enviar para MASTER***

git flow finish --push  (ESQ :wq)

git flow release finish v1.33.0

##

:w esse aqui vai salvar a adição

:q esse aqui vai fechar o vi

:q! esse aqui vai forçar o fechamento do vi (muito util quando não tem permissão de alterar o arquivo)

:wq esse aqui é a junção do salvar com o sair...

