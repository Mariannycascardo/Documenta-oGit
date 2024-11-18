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
##### Adicionar um Repositório Local ao GitHub:

```dart
git init
git remote add origin <URL-do-repositório>
git add .
git commit -m "Primeiro commit"
git push -u origin main
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


### GitHub

##### é uma plataforma de hospedagem de código que utiliza o sistema de controle de versão Git. Ele permite que desenvolvedores trabalhem juntos em projetos de forma colaborativa e eficiente. 

#### Funcionalidades Principais

##### *Repositórios:*

##### Espaços onde todo o código-fonte de um projeto é armazenado. Podem ser públicos (visíveis a todos) ou privados (restritos a usuários específicos).

##### *Branches:*

##### Ramificações que permitem desenvolver novas funcionalidades ou corrigir bugs sem interferir na versão principal (geralmente chamada de main ou master).

##### *Commits:*
##### Alterações no código com mensagens descritivas, ajudando a documentar o que foi modificado.

##### *Pull Requests (PR):*

##### Ferramentas para discutir e revisar alterações propostas antes de serem mescladas com a branch principal.

##### *Issues:*

##### Permitem o rastreamento de tarefas, bugs e solicitações de recursos, funcionando como um sistema de gerenciamento de projetos.

##### *GitHub Actions:*

##### Serviço de CI/CD que permite automatizar fluxos de trabalho de desenvolvimento, como testes e deploys.

##### *Wikis:*

##### Ferramenta de documentação colaborativa, permitindo que projetos tenham uma área dedicada a guias e instruções.

#### Como Usar o GitHub



##### *Login:*

##### Acesse sua conta no GitHub em github.com.

##### Novo Repositório:

- ##### Clique em New repository.

- ##### Dê um nome ao repositório, adicione uma descrição opcional e defina a visibilidade (pública ou privada).

- ##### Clique em Create repository.

#### Conectar Repositório Local

##### Inicialize um repositório Git local:

```dart
git init
```

##### Conecte ao repositório remoto:
```dart
git remote add origin <URL-do-repositório>
```

#### Enviar Código para o GitHub

##### Adicione arquivos ao stage:

```dart
git add .
```

##### Faça commit das alterações:

```dart
git commit -m "Mensagem do commit"
```
##### Envie as alterações para o GitHub:

```dart
git push origin main
```

#### Colaboração em Projetos

##### *Forks:* 

##### Crie uma cópia de um repositório para trabalhar em seu próprio espaço antes de propor mudanças ao repositório original.

##### *Branches:*

##### Crie branches específicas para cada tarefa, como feature/novo-recurso ou fix/corrigir-bug.

##### *Revisão de Código:*

##### Use PRs para revisões, permitindo comentários e sugestões de outros colaboradores antes de mesclar as mudanças.

#### GitHub Pages

##### *Hospedagem Gratuita de Sites:*

##### Permite que você publique páginas web diretamente a partir de um repositório.

##### *Uso*

##### Configure a branch gh-pages ou use uma pasta /docs no repositório para hospedar conteúdos como portfólios e documentações.

####  GitHub Actions

##### *Automação de Fluxos de Trabalho*

- ##### Escreva scripts em YAML para definir processos automáticos, como testes de código e implantações.

##### Exemplo de um workflow:
```dart
name: Build and Test
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Run Tests
        run: npm test
```

#### Segurança e Controle de Acesso

- ##### Repositórios Privados e Públicos: Escolha a visibilidade de cada repositório.

- ##### Proteção de Branches: Configure regras para proteger branches críticas (ex.: main), exigindo revisões antes de mesclar PRs.

- ##### Autenticação de Dois Fatores (2FA): Adicione uma camada extra de segurança à sua conta GitHub.

#### Integrações e Ferramentas

##### GitHub CLI: Interface de linha de comando que permite gerenciar repositórios diretamente do terminal.

##### APIs: O GitHub oferece APIs que permitem automatizar tarefas e acessar informações do repositório programaticamente.

##### Extensões de IDE: Integre o GitHub a editores de código como Visual Studio Code para facilitar commits, pushes e pull requests.

#### Dicas de Boas Práticas

- ##### Commits Pequenos e Descritivos: Facilitam o rastreamento de alterações.

- ##### Branches Nomeadas de Forma Clara: Use nomes descritivos, como feature/novo-recurso ou fix/erro-login.

- ##### Documentação Detalhada: Sempre inclua um README.md com informações sobre o projeto e um CONTRIBUTING.md para diretrizes de colaboração.

#### Git Bash

##### O que é Git Bash?

##### É um terminal de linha de comando para sistemas Windows que permite aos desenvolvedores interagir com o Git, utilizando comandos do Bash típicos de sistemas Unix/Linux. Ele oferece uma interface que emula o comportamento de um shell Bash no Windows, permitindo o uso de comandos Git diretamente, bem como ferramentas e utilitários de linha de comando similares aos encontrados em sistemas Unix.

#### Instalação do Git Bash

- ##### Sistema Operacional: Windows 7 ou superior

- ##### Conexão à internet para download do instalador.

#### Passos para Instalação 

##### Acesse o site oficial do Git (git-scm.com) e baixe o instalador adequado para o seu sistema Windows.

##### Execute o arquivo de instalação baixado.

##### Durante o processo de instalação, selecione as opções padrão recomendadas, a menos que você tenha requisitos específicos.

##### No momento da escolha de componentes, certifique-se de que a opção Git Bash esteja selecionada.

##### Complete a instalação e, ao final, o Git Bash estará disponível no menu Iniciar do Windows.

#### Comandos Básicos do Git Bash

##### O Git Bash permite o uso de comandos nativos do Linux/Unix e do Git. Abaixo estão alguns dos comandos mais utilizados:

##### Comandos de Navegação e Manipulação de Arquivos

- ##### pwd: Exibe o caminho do diretório atual.

- ##### ls: Lista os arquivos e pastas no diretório atual.

- ##### cd <diretório>: Navega até o diretório especificado.

- ##### mkdir <nome_do_diretorio>: Cria um novo diretório.

- ##### rm <arquivo>: Remove um arquivo.

- ##### cp <origem> <destino>: Copia um arquivo ou diretório.

- ##### mv <origem> <destino>: Move ou renomeia um arquivo ou diretório.

#### Comandos de Utilitário

##### O Git Bash oferece suporte a muitos comandos Unix tradicionais:

- ##### grep: Pesquisa por padrões em um arquivo.

- ##### sed: Editor de fluxo para manipulação de texto.

- ##### awk: Processamento de texto e dados em arquivos.

- ##### ssh: Conecta-se a servidores via SSH.

##### Comandos Bash Tradicionais

- ##### Comandos de navegação e manipulação de arquivos: cd, ls, cp, mv, rm, cat.

- ##### Comandos de controle de fluxo e scripts: if, for, while, case.

 - ##### Redirecionamento de entradas e saídas: Usar >, >>, | para redirecionar e canalizar dados.

#### Criando um Repositório no GitHub

##### Acesse sua conta do GitHub e clique em "New Repository".

##### Dê um nome ao repositório, por exemplo, meu-projeto.

##### Defina as opções do repositório:

- ##### Escolha entre público ou privado.

- ##### Adicione um README.md, se desejar.

- ##### Clique em "Create repository".

#### Preparando o Projeto Localmente

##### Navegue até o diretório do projeto no seu computador:

```dart
cd caminho/para/seu-projeto
```

##### Inicialize um repositório Git, caso ainda não tenha feito:

```dart
git init
```

##### Adicione o repositório remoto do GitHub ao projeto:

```dart
git remote add origin https://github.com/seu-usuario/meu-projeto.git
``` 
#### Versionando e Preparando Arquivos para o Commit

##### Adicione os arquivos ao "staging area":

```dart 
git add .
```
##### Verifique os arquivos que foram adicionados:

```dart
git status
```
##### Crie um commit com uma mensagem descritiva:

```dart
git commit -m "Primeiro commit - adicionando todos os arquivos do projeto"
```

####  Subindo a Aplicação para o Repositório

##### Envie os arquivos para o repositório remoto:

```dart
git push -u origin main
```
- ##### Nota: Se o nome da branch principal for master, substitua main por master.

#### Solução de Problemas Comuns

- ##### Erro de autenticação: Se você encontrar um erro de autenticação, verifique se está usando um token de acesso pessoal em vez de senha. Configure-o no GitHub em Settings > Developer settings > Personal access tokens.

- ##### Branch desatualizada: Se houver atualizações no repositório remoto, você precisará fazer git pull origin main antes de empurrar novamente.

- ##### Erro de branch divergente: Use git pull --rebase origin main para alinhar a branch local com a remota.

####  Passos Adicionais e Boas Práticas

- ##### Atualize o arquivo README.md para incluir uma descrição clara do projeto.

- ##### Adicione um .gitignore para evitar subir arquivos desnecessários, como logs ou pastas de configuração local.

- ##### Verifique o repositório remoto no GitHub para garantir que todos os arquivos e pastas foram corretamente enviados.

####  Subindo Atualizações Futuras

##### Sempre que fizer modificações no projeto e quiser enviar atualizações:

##### Adicione as alterações:

```dart
git add .
```

##### Crie um novo commit:

```dart
git commit -m "Descrição das alterações"
```
##### Envie as atualizações:

```dart
git push origin main
```





















