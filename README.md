# Workspace GitHub e Git Flow

## Git

O Git é um sistema de controle de versão distribuído amplamente usado na área de desenvolvimento de software. Ele permite que você rastreie e gerencie alterações em arquivos, crie ramificações para desenvolver recursos independentes e mescle essas mudanças de forma eficiente. É uma ferramenta fundamental para o desenvolvimento colaborativo, ajudando a manter o código organizado e permitindo o trabalho em equipe de maneira eficaz.

## Gitflow

Gitflow é um modelo de fluxo de trabalho que busca simplificar e organizar o versionamento de ramificações de um projeto de desenvolvimento no Git.

**Main:** é a ramificação principal que contém o código-fonte em produção. Não é permitido realizar alterações (commit) diretamente nessa ramificação. A Master ainda é utilizada para enviar os commits dos releases para a produção;

**Develop:** criada a partir da ramificação Main, ela reúne os códigos de todos os ramos e se comunica com a Main. Ela contém o código-fonte mais atual e todas as novas features estáveis que serão mescladas posteriormente;

**Feature:** criada a partir da ramificação Develop, é uma branch temporária que carrega uma nova funcionalidade para o projeto, ela sempre acabará sendo mesclada à própria Develop através de merge. E segue um padrão de nomenclatura “feature/new-feature”.

**Release:** é uma ramificação temporária que fará com que os novos recursos armazenados na Develop sejam mesclados na branch Master, recebendo uma tag que indica a nova versão do projeto.

**Hotfix:** é uma ramificação utilizada para mesclar correções na ramificação principal decorrente de bugs identificados no processo de desenvolvimento. Após a correção do bug, o código irá tanto para a branch main como para a Develop. Essa branch também recebe uma tag indicando a nova versão na Main.


## Criando um repositorio



## Clonando um Repositório



## Branchs

![branch-feature](./img/image.png)


## Commits



## Comandos Básicos

### Git init
inicializa um repositório Git dentro de um diretório do sistema.

> git init

### Git clone
cria uma cópia de um repositório remoto em um diretório da máquina.

> git clone *(https://github.com/(userGitHub)/(repositoryName).git)*

### Git status
verifica o status do git atualmente. Esse comando mostra se o projeto local está sincronizado com o master, quais arquivos estão sendo monitorados pelo Git e em qual branch você está. 

> git status

### Git add
adiciona arquivos ao pacote de alterações para serem feitas. É possível adicionar um arquivo ou múltiplos arquivos por vez.

> git add <-arquivo1->

**Observação:** Adiciona somente o arquivo 1 para o pacote.

> git add . 

**Observação:** Adiciona todos os arquivos modificados ao pacote.

### Git commit
etapa crucial para registrar uma nova versão do projeto, composta por um conjunto de alterações. Ele pega as modificações que foram adicionadas usando o comando git add, agrupa essas mudanças em um conjunto e as identifica com um código único chamado Hashcode. Além disso, em cada commit, é necessário incluir uma mensagem descritiva que esclareça quais foram as alterações feitas nessa atualização. Isso torna mais fácil entender o propósito e o conteúdo de cada commit no histórico do projeto.

> git commit -m "Adicionando cards"

### Git branch
cria novas branchs de desenvolvimento, bem como visualiza quais são os ramos existentes. 

> git branch

> git branch feature/cards

> git checkout: navegar entre as branchs do projeto. 

> git checkout feature/cards