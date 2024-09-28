# 📝Lista de Comandos do Git:

# Configurações Globais
- $ git config --global user.name "nome" → Configura o nome do usuário para os commits.
- $ git config --global user.email "email" → Configura o e-mail do usuário para os commits.

# Inicializando e Verificando o Repositório
- $ git init → Inicializa um novo repositório Git.
- $ git status → Exibe o status atual do repositório.

# Adicionando Arquivos
- $ git add "arquivo" → Adiciona um arquivo à área de staging.
- $ git add . → Adiciona todos os arquivos modificados à área de staging.

# Commitando Mudanças
- $ git commit –m “msg..." → Cria um commit com uma mensagem.
- $ git commit -am “msg..." → Adiciona e commit todos os arquivos modificados.

# Básicos
- $ git log → Mostra o histórico de commits.
- $ git remote add origin "link" → Conecta o repositório local a um repositório remoto.
- $ git push origin master → Envia as alterações para o branch master do remoto.
- $ git clone "link" → Clona um repositório remoto para o local.

# Visualizando Histórico
- $ git log → Exibe o histórico de commits no repositório.
- $ git log –n 1 → Mostra o último commit.
- $ git log --oneline → Exibe o histórico de commits em uma linha por commit.
- $ git log -n 1 --oneline → Mostra o último commit de forma simplificada.

# Comparando Diferenças
- $ git diff → Exibe as diferenças entre o código atual e o último commit.
- $ git diff --staged → Mostra as diferenças dos arquivos na área de staging.
- $ git diff 9167ba → Compara o estado atual com o commit identificado pelo hash 9167ba.

# Removendo e Movendo Arquivos
- $ git rm "arq.arq" → Remove um arquivo do repositório e da área de staging.
- $ git mv → Move ou renomeia um arquivo.

# Revertendo e Resetando
- $ git checkout -- nomeDoArquivo → Reverte as mudanças no arquivo para o último commit.
- $ git reset -- arquivo → Remove o arquivo da área de staging.
- $ git reset --hard → Desfaz todas as mudanças locais, voltando ao último commit.
- $ git reset --hard 7b750f3 → Reseta o repositório para o estado de um commit específico.
- $ git revert --no-edit 7b750f3 → Reverte um commit específico, criando um commit inverso.

# Manipulação de Remotos
- $ git fetch → Baixa atualizações do repositório remoto.
- $ git diff ...origin → Compara as diferenças entre o branch local e o remoto.
- $ git pull → Puxa e mescla as alterações do remoto com o branch local.
- $ git pull origin master → Puxa e mescla as mudanças do branch master no repositório remoto
- $ git remote -v → Lista os repositórios remotos configurados.
- $ git remote rm → Remove um repositório remoto.

# Branches
- $ git branch → Lista todas as branches.
- $ git branch "novaBranch" → Cria uma nova branch.
- $ git branch –v → Exibe o último commit de cada branch.
- $ git checkout "nome" → Muda para a branch especificada.
- $ git checkout -b "nome" → Cria e muda para uma nova branch.
- $ git branch -d "nome" → Deleta uma branch local.
- $ git branch -D "nome" → Força a exclusão de uma branch.
- $ git branch --no-merged → Lista as branches que não foram mescladas.
- $ git branch --merged → Lista as branches já mescladas.

# Mesclagem e Rebasing
- $ git merge "arquivo" -m "msg..." → Mescla uma branch no branch atual com uma mensagem de merge.
- $ git log -n 5 --oneline --decorate --parents → Mostra os últimos 5 commits com informações de merge.
- $ git rebase "nome" → Rebaseia a branch atual em cima de outra branch.

# Histórico e Revisões
- $ git reflog → Mostra o histórico de todas as ações, incluindo resets.
- $ git reset HEAD@{3} --hard → Reseta o repositório para um estado anterior usando o reflog.

# Comandos do Sistema
- $ ls -l → Lista arquivos no diretório com detalhes.
- $ ls -lha → Lista arquivos, incluindo ocultos, com tamanhos legíveis.
- $ mkdir nome_do_arquivo → Cria um novo diretório.

# Extra
- $ git stash → Salva temporariamente as mudanças não commitadas para você trabalhar em outra coisa e depois restaurá-las.
- $ git stash apply → Aplica as mudanças armazenadas com git stash ao seu diretório de trabalho.
- $ git stash pop → Aplica as mudanças e remove o stash da lista.
- $ git tag "v1.0" → Marca um ponto específico no histórico, como um lançamento de versão.
- $ git tag -a "v1.0" -m "Versão 1.0" → Cria uma tag anotada com uma mensagem.
- $ git show "tag" → Mostra os detalhes de uma tag específica ou commit.
- $ git cherry-pick "hash" → Aplica um commit específico de outro branch ao seu branch atual.
- $ git shortlog → Resumo dos commits agrupados por autor.
- $ git clean -f → Remove arquivos não rastreados do diretório de trabalho.
- $ git blame "arquivo" → Mostra quem fez cada alteração em um arquivo linha por linha.
