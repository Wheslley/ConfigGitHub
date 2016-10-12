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
    
# Sobrescrever alterações locais

    git checkout -- <arquivo>
    
# Sobrescrever todo o diretorio

    git fetch origin
    git reset --hard origin/master
    
# Inclusões interativas

    git add -i
