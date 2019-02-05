2. Git Commands
============

_Uma lista de comandos comuns usados no Git_

--

### Clonando & Criando Projetos

| Comando | Descrição |
| ------- | ----------- |
| `git init` | Inicializa um repositório local de Git |
| `git clone https://github.com/[username]/[repository-name].git` | Cria uma cópia local (clone) de um repositório remoto |

### Operações básicas

| Comando | Descrição |
| ------- | ----------- |
| `git status` | Checa o status |
| `git add [file-name.txt]` | Adiciona um arquivo à área de staging |
| `git add -A` | Adiciona todos os arquivos novos e que foram alterados à área de staging |
| `git commit -m "[commit message]"` | Commit as mudanças |
| `git rm -r [file-name.txt]` | Remove um arquivo ou pasta |

### Branching & Merging

| Comandos | Descrição |
| ------- | ----------- |
| `git branch` | Lista branches (o asterisco marca o branch atual) |
| `git branch -a` | Lista todos os branches (local e remoto) |
| `git branch [branch name]` | Cria um novo branch |
| `git branch -d [branch name]` | Deleta um branch |
| `git push origin --delete [branchName]` | Deleta um branch remoto |
| `git checkout -b [branch name]` | Cria um novo branch e passa a usá-lo |
| `git checkout -b [branch name] origin/[branch name]` | Clona um branch remoto e passa a usá-lo |
| `git checkout [branch name]` | Usar o branch como destino dos commits |
| `git merge [branch name]` | Merge um branch em um branch ativo (branch atual)|
| `git merge [source branch] [target branch]` | Merge um branch com um outro branch |
| `git stash` | Fazer Stash nas mudanças em um diretorio para trabalhar em outro branch, sem precisar commit |
| `git stash clear` | Remove todas as entradas de stashed |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Envia os arquivos do branch para o repositórop remoto |
| `git push -u origin [branch name]` | Envia os arquivos do branch para o repositórop remoto (e mantém o branch) |
| `git push` | Envia os arquivos do branch para o repositórop remoto (no branch ativo) |
| `git push origin --delete [branch name]` | Deleta um brach remoto
| `git pull` | Atualiza os arquivos locais pelos arquivos do repositório remoto (download) |
| `git pull origin [branch name]` | Faz o download das mudanças de um repositório remoto |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Adicionar um repositório remoto |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Configura um repositório remoto para ser acesado por SSH |

### Inspeção & Comparação

| Comando | Descrição |
| ------- | ----------- |
| `git log` | Visualizar mudanças |
| `git log --summary` | Visuaizar detalhadamenteo as mudanças |
| `git diff [source branch] [target branch}` | Pre-visualizar as mudanças antes de um merge |

