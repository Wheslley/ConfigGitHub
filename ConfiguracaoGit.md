# Instalar o Git

	https://git-scm.com/downloads

# Configurar email e username

	git config --global user.email "seu_email@dominio.com"
	git config --global user.name "seu_username"

# Configurar Git e Git Hub

 $ Gerar uma chave ssh
 
 	ssh-keygen -t rsa -b 4096 -C "seu_email@dominio.com"
	OBS: Não é necessário colocar senha. Lembrando que será solicitado a senha sempre que for submeter algum commit para o repositório.
	
 $ Ativar o ssh-agent e associar uma chave ssh a ele
 
	exec ssh-agent bash
	ssh-add ~/.ssh/id_rsa
	
 $ Copiar a chave gerada e associar ao Git Hub
 
	clip < ~/.ssh/id_rsa.pub
	Entrar no site Git Hub > Settings > SSH and GPG keys > New SSH key
		Title: Colocar qualquer nome para sua chave ssh
	 Key: Apenas dê um ctrl+v
	 
 $ Testar Git e Git Hub
 
	ssh -T git@github.com
	yes
	OBS: A mensagem deverá ser um "Hi seu_user! ... " (Caso não seja, repita os procedimentos acima).
	
 $ Excluir e Setar Keys Git
 
 	ssh-add -D
	ssh-add yourKey
	ssh -T git@github.com
