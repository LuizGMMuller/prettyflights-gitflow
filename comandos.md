# Comandos Git

## 1. Inicialização e Configuração

---

### git init

Inicializa um novo repositório Git local.

#### Exemplos

```bash
git init
git init meu-projeto
git config

Define configurações do Git, como nome e email do usuário.

Exemplos
git config --global user.name "Luiz"
git config --global user.email "luiz@email.com"
git clone

Cria uma cópia local de um repositório remoto.

Exemplos
git clone https://github.com/user/repositorio.git
git clone https://github.com/user/repositorio.git projeto-local
git remote

Gerencia repositórios remotos associados ao projeto.

Exemplos
git remote -v
git remote add origin https://github.com/user/repositorio.git
2. Manipulação de Arquivos
git status

Mostra o estado atual do repositório.

Exemplos
git status
git status -s
git add

Adiciona arquivos para a área de stage.

Exemplos
git add arquivo.txt
git add .
git commit

Salva as alterações adicionadas no histórico do Git.

Exemplos
git commit -m "feat: adiciona tela de login"
git commit -m "fix: corrige erro no check-in"
git rm

Remove arquivos do repositório.

Exemplos
git rm arquivo.txt
git rm -r pasta/
git mv

Move ou renomeia arquivos rastreados pelo Git.

Exemplos
git mv antigo.txt novo.txt
git mv pasta1/arquivo.txt pasta2/
3. Branches e Integração
git branch

Cria ou lista branches.

Exemplos
git branch
git branch feature/login
git checkout

Troca de branch ou restaura arquivos.

Exemplos
git checkout develop
git checkout -b feature/checkin
git switch

Alternativa moderna para troca de branches.

Exemplos
git switch main
git switch -c release/1.0.0
git merge

Integra mudanças entre branches.

Exemplos
git merge develop
git merge hotfix/1.0.1
git rebase

Reorganiza commits aplicando-os sobre outra base.

Exemplos
git rebase main
git rebase develop
4. Histórico e Inspeção
git log

Exibe o histórico de commits.

Exemplos
git log
git log --oneline
git diff

Mostra diferenças entre versões de arquivos.

Exemplos
git diff
git diff main develop
git show

Exibe detalhes de commits específicos.

Exemplos
git show
git show HEAD
git blame

Mostra quem alterou cada linha de um arquivo.

Exemplos
git blame app.js
git blame README.md
5. Repositórios Remotos
git push

Envia commits locais para o repositório remoto.

Exemplos
git push origin main
git push -u origin develop
git pull

Baixa e integra alterações do repositório remoto.

Exemplos
git pull origin main
git pull
git fetch

Baixa alterações do remoto sem integrar automaticamente.

Exemplos
git fetch origin
git fetch --all
6. Correções e Recuperação
git reset

Remove commits ou alterações da área de stage.

Exemplos
git reset HEAD arquivo.txt
git reset --hard HEAD~1
git revert

Cria um commit que desfaz alterações anteriores.

Exemplos
git revert HEAD
git revert a1b2c3d
git stash

Armazena alterações temporariamente.

Exemplos
git stash
git stash pop
7. Tags e Versionamento
git tag

Cria marcações de versão no histórico do projeto.

Exemplos
git tag v1.0.0
git tag -a v1.0.1 -m "Versão 1.0.1"
git describe

Mostra informações sobre tags e commits.

Exemplos
git describe
git describe --tags
8. Trabalho Colaborativo
git cherry-pick

Aplica commits específicos de outra branch.

Exemplos
git cherry-pick a1b2c3d
git cherry-pick HEAD~1
git restore

Restaura arquivos para um estado anterior.

Exemplos
git restore arquivo.txt
git restore --staged arquivo.txt