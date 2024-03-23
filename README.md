-> Criar o repositório no próprio site do github

Cadastrar uma chave SSH no Github para dar acesso ao computador

Comandos para configurar a identificação no github (precisa fazer apenas 1x no computador)
git config --global user.name "Seu nome"
git config --global user.email "Seu email de cadastro do Github"
git config --list

-> Trocando uma versão antiga de autenticacao (URL) pela chave SSH:
git remote -v 					para listar qual esta cadastrado, se estiver cadastrado uma https://... trocar para ssh
git remote remove name			ex: git remote remove origin
git remote add origin git@github.com:seuusuario/seurepositorio.git		

Caso ao tentar dar push aparecer a mensagem pedindo para dar "git push --set-upstream origin main", usar o comando no terminal e dar o push em seguida, ou usar git push -u origin main


-> Salvando a primeira versão do repositório (dando push pela primeira vez de um repositório local para o remoto recem criado)
git init
git add .
git commit -m "Mensagem explicativa"
git branch -M main
git remote add origin git@github.com:seuusuario/seurepositorio.git
git push -u origin main

-> Salvando novas versões ( dando push após já ter dado algum push antes )
git status
git add .
git commit -m "Mensagem explicativa"
git push


-> Clonando um repositório
git clone git@github.com:seuusuario/seurepositorio.git
git add .
git commit -m "Mensagem explicativa"
git push



-> Verificando o histórico de versões
git log
git log --oneline


git diff
• Comando que mostra a diferença entre arquivos modificados
• Dica: utilizar o VS Code, que mostra graficamente as diferenças

git remote -v
git remote remove name
git remote add origin git@github.com:seuusuario/seurepositorio.git

git checkout
(incompleto) 
