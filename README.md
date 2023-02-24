# Curso-de-Git

Curso de GIT 23/02/2023

-------------------------------------------------------------
- Ferramenta de controle de versão
- Gerenciamento por linha de comando

-------------------------------------------------------------
		Configuramos o GIT  no Git Bash
Comandos:
$ git config --global user.name"nome" -> seta o nome
$ git config --global user.email"email" -> seta o email

-------------------------------------------------------------                      
Como utilizar o GIT para o controle de projetos

Alterar pasta para repositorio -> pelas propriedades do Windows, mudando o "iniciar em"

Comandos:
cd -> acessa uma pasta
cd .. -> volta uma pasta
clear -> limpar a dash
Criar repositorio -> git init -> cria uma pasta invisivel ao explorer, mas esta lá
git status -> status atual de seu repositorio 
obs... Adicionamos nossos arquivos na nossa pasta de git para começar a fazer o controle deles
Para adicionar arquivo a ser monitorado pelo git usamos ------>  git add "nome do arquivo e a extensao sem aspas"
ou git add"*.extensao" para adicionar tudo da extensao
ou git add "." para adicionar toda a pasta

git add -> passamos os arquivos para a area de espera, precisamos confirmar o projeto

Comando:
git commit -m "Teste1" -> salva mudanças e denifine um nome para o salvamento
Para o git ignorar um arquivo -> criamos novo arquivo chamado".gitignore" e colocamos os arquivos lá

git commit -a -m "Teste1" -> salva mudanças e pula etapa da area de espera

-------------------------------------------------------------
git diff -> Para consultar as alterações nos arquivos digitamos 
git diff --staged -> Consultar arquivos na area de espera
git log -> mostra todos os commits feitos em nosso programa
git log -p -> Mostra todas as linhas dos programas por paginação (Letra Q volta no terminal normal)
git log -p (- "Especificar quantas linhas você deseja")
git log --pretty=oneline -> Mostra o codigo e a mensagem de cada commit
Interface Gráfica:
gitk -> Para visualizarmos na interface grafica todas as alterações feitas

-------------------------------------------------------------
				Revertendo Situações:

Para editar um commit:
{  -> simbolico
git add -> para adicionarmos o arquivo a ser editado
git commit --ammend -m "nome da alteração" (edição - pode trocar o nome)
}

git checkout -- (Nome do arquivo) -> Para restaurar um arquivo modificado

Para remover arquivos:
git rm (nome do arquivo)

md -> cria nova pasta

-------------------------------------------------------------

				CRIANDO TAGS

Uma tag ajuda a reverter, consultar arquivo antigo

Criando -> git tag -a ("Nome da tag") -m ("Podemos incluir uma mensagem aqui")
ex:
git tag -a v1.0 -m "Versao 1.0"

git tag -> mostra a versao que estamos, no caso nossa tag
git show -> mostra os detalhes da tag que estamos ou se especificado a tag mostra detalhes da tag especificada
git checkout -> faz a troca da tag pro ponteiro inicial, troca os arquivos
git tag -d (nome da tag a ser deletada) -> deleta a tag

-------------------------------------------------------------
					BRANCH
git branch (nome do branch) -> cria um branch
git checkout teste -> transfere arquivos para o branch

ou o comando
git chechout -b (nome do branch) -> Realiza as duas linhas de cima de uma só vez

Comitamos o branch pra implementar e utilizamos o comando ->
git merge (nome do branch)

git branch -d (nome do branch) -> teleta branch de teste

-------------------------------------------------------------
					GITHUB
ssh-keygen -> gera par de chaves ssh
git clone (repositorio)-> clona repositorio (baixa ele pra maquina)
git push origin master -> enviar arquivos pro repositorio
git push -> transfere commits do repositório local a um repositório remoto

-------------------------------------------------------------
