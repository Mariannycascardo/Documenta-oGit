# *Documentação do Git*

### Git

#### O que é Git?

##### Git é um sistema de controle de versão distribuído, criado por Linus Torvalds em 2005, projetado para rastrear mudanças em arquivos de código-fonte e facilitar o trabalho colaborativo em projetos de software. É amplamente usado devido à sua eficiência, flexibilidade e suporte robusto a projetos em equipe.

#### Conceitos Fundamentais do Git

##### Repositório (Repository):

- ##### É um local onde o histórico de versões de um projeto é armazenado. Pode ser local (no seu computador) ou remoto (em plataformas como GitHub, GitLab ou Bitbucket).

##### Commit:

- ##### Um ponto de verificação no histórico do projeto, contendo um instantâneo das alterações feitas nos arquivos.

##### Branch: 

- ##### Uma linha separada de desenvolvimento que permite criar e trabalhar em novas funcionalidades ou correções sem afetar a main (ou master).

##### Merge:

- ##### Combina alterações de uma branch em outra. Pode gerar conflitos que precisam ser resolvidos manualmente.

##### Staging Area:

- ##### Uma área onde as alterações são preparadas antes de serem confirmadas com um commit.

##### Push e Pull:

- ##### Push: Envia alterações do repositório local para o repositório remoto. 

- ##### Pull: Puxa as alterações do repositório remoto para o repositório local.

##### Clone:

- ##### Copia um repositório remoto para o seu computador, criando uma cópia completa com todo o histórico de versões. 

### Comandos Essenciais do Git

##### Inicializar um Repositório: 

```dart
git init

```
##### Clonar um Repositório Remoto

```dart
git clone <URL-do-repositório>
```
##### Adicionar Arquivos ao Stage:

```dart
git add arquivo.txt
git add . # Adiciona todos os arquivos modificados
```
##### Fazer um Commit:

```dart
git commit -m "Mensagem descritiva do commit"
```
##### Verificar o Status dos Arquivos:

```dart
git status
```
##### Criar uma Nova Branch:

```dart
git branch nova-branch

```
##### Trocar para uma Branch:

```dart
git checkout nova-branch
```
##### Combinar Branches:

```dart
git merge nova-branch
```
##### Enviar Mudanças para o Repositório Remoto:

```dart
git push origin main
```
##### Puxar Atualizações do Repositório Remoto:

```dart
git pull origin main
```
#### Conceitos Avançados

##### Rebase:

##### Reaplica commits de uma branch em outra para criar um histórico de commits mais linear.

```dart
git rebase main
```

##### Stash:

##### Salva temporariamente mudanças não confirmadas e limpa o diretório de trabalho.

```dart
git stash
git stash pop # Recupera as mudanças salvas
```
##### Cherry-pick

##### Aplica um commit específico de uma branch em outra.

```dart
git cherry-pick <commit-hash>
```
#### Comandos Básicos


- ##### git init: Inicializa um novo repositório Git no diretório atual.

- ##### git clone URL: Clona um repositório remoto para o seu computador.

- ##### git status: Mostra o estado atual do repositório (quais arquivos foram modificados, quais estão no stage, etc.).

- ##### git add arquivo: Adiciona arquivos ao stage para preparar para commit.

- ##### git add . : Adiciona todos os arquivos modificados ao stage.

- ##### git commit -m "mensagem" : Cria um commit com as mudanças no stage e uma mensagem descritiva.

- ##### git push origin branch: Envia os commits locais para o repositório remoto.

- ##### git pull: Baixa as alterações do repositório remoto e faz o merge com a branch local. 

- ##### git branch: Lista todas as branches no repositório.

- ##### git branch nome: Cria uma nova branch.

- ##### git checkout branch: Alterna para a branch especificada.

- ##### git switch branch: Alternativa moderna ao checkout para mudar de branch.

- ##### git merge branch: Faz merge das alterações de uma branch na branch atual.

- ##### git remote add origin URL: Conecta o repositório local a um repositório remoto.

#### Comandos para Visualização e Histórico

- ##### git log: Mostra o histórico de commits.

- ##### git log --oneline: Exibe o histórico de commits de forma compacta (em uma linha).

- ##### git diff: Mostra as diferenças entre arquivos modificados que ainda não foram colocados no stage.

- ##### git show commit: Mostra as alterações feitas em um commit específico.

#### Comandos de Controle de Branches

- ##### git branch -d branch: Deleta uma branch local.

- ##### git branch -m nome-antigo novo-nome: Renomeia uma branch.

- ##### git checkout -b branch: Cria uma nova branch e muda para ela imediatamente.

#### Comandos Avançados

- ##### git stash: Salva temporariamente as alterações locais não commitadas.

- ##### git stash pop: Restaura as alterações salvas e as remove da pilha.

- ##### git rebase branch: Aplica commits de uma branch em outra, reestruturando o histórico.

- ##### git cherry-pick commit: Aplica um commit específico de uma branch em outra.

#### Comandos para Repositórios Remotos

- ##### git fetch: Puxa atualizações do repositório remoto sem fazer merge.

- ##### git remote -v: Lista as URLs do repositório remoto.

- ##### git pull origin branch: Puxa as alterações de uma branch específica do remoto.

#### Comandos de Configuração

- ##### git config --global user.name "Seu Nome": Define o nome de usuário globalmente.

- ##### git config --global user.email "seuemail@exemplo.com": Define o e-mail do usuário globalmente.

#### Comandos de Tags

- ##### git tag nome-da-tag: Cria uma tag para marcar um commit específico.

- ##### git tag: Lista todas as tags no repositório.

#### Comandos de Limpeza e Revisão

- ##### git clean -f: Remove arquivos não rastreados do diretório de trabalho.

- ##### git reset arquivo: Remove o arquivo do stage.

- ##### git reset --hard: Restaura o repositório para o último commit, removendo todas as alterações.












### Git Hub

#### Visão Geral

##### GitHub é uma plataforma de hospedagem de código que permite gerenciar repositórios, colaborar e compartilhar projetos com outras pessoas.

#### Instalação

##### Criar Conta: Acesse github.com e crie uma conta gratuita.

##### Instalar Git: Baixe e instale o Git.

##### Configurar Git: Defina seu nome e e-mail no Git Bash:

```dart
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
```
##### Clonar Repositório: Para projetos existentes, use:

```dart
git clone <URL-do-repositório>
```

### Git Bash 

#### Visão Geral

##### Git Bash é um terminal que emula o ambiente de comando do Git em sistemas Windows, permitindo o uso de comandos Git e Unix, como ls, cd e rm. Ele facilita o uso do Git em ambientes que normalmente não têm acesso a comandos Unix.

#### Instalação

##### Baixe o Git Bash em git-scm.com para Windows.
##### Instale o software e selecione o Git Bash como opção de terminal durante a instalação.

#### Uso

 ##### Com o Git Bash, você pode usar os principais comandos Git e Unix:
- ##### Comandos básicos do Git: git init, git add, git commit, git push, entre outros.
- ##### Comandos Unix:
- ##### Navegação: cd <pasta>, ls
- ##### Manipulação de arquivos: cp, mv, rm

#### Exemplos


##### Criar uma nova pasta e entrar nela:

```dart
mkdir novo_projeto
cd novo_projeto
```

##### Clonar um repositório Git:

```dart
git clone <URL>
```
##### Verificar o status do repositório:

```dart
git status`
```
### Subir as aplicações 

