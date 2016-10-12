# Criando um novo diretório

    git init

# Obtenha um repositório em um repositório local

    git clone /caminho/para/o/repositorio

# Adicionar arquivo

    git add <arquivo> 
    git add *
    
# Confirmar mudanças

    git commit -m "comentários das alterações"
    
# Enviando alterações

    git push origin master --force
    
# Atualizar seu diretório

    git pull
    
# Para mesclar seu diretório

    git merge <branch>
    
# Para visualizar conflitos

    git diff <branch origem> <branch destino>
    
# Visualisar logs

    git log

# Visualisar logs gráficos

    gitk
    
# Sobrescrever alterações locais

    git checkout -- <arquivo>
    
# Sobrescrever todo o diretorio

    git fetch origin
    git reset --hard origin/master
    
# Inclusões interativas

    git add -i

# Atualizar o fork com o master

    git remote add upstream https://github.com/usuario/projeto.git

    git fetch upstream

    git checkout master

    git rebase upstream/master

    git merge upstream/master

    git push -f origin master