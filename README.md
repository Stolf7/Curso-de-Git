# Curso-de-Git

Curso de GIT 23/02/2023</br>

-------------------------------------------------------------</br>
- Ferramenta de controle de versão</br></br>
- Gerenciamento por linha de comando</br>

-------------------------------------------------------------</br>
		Configuramos o GIT  no Git Bash</br>
Comandos:</br>
$ git config --global user.name"nome" -> seta o nome</br>
$ git config --global user.email"email" -> seta o email</br>

-------------------------------------------------------------  </br>                    
Como utilizar o GIT para o controle de projetos</br>

Alterar pasta para repositorio -> pelas propriedades do Windows, mudando o "iniciar em"</br>

Comandos:</br>
cd -> acessa uma pasta</br>
cd .. -> volta uma pasta</br>
clear -> limpar a dash</br>
Criar repositorio -> git init -> cria uma pasta invisivel ao explorer, mas esta lá</br>
git status -> status atual de seu repositorio </br>
obs... Adicionamos nossos arquivos na nossa pasta de git para começar a fazer o controle deles</br>
Para adicionar arquivo a ser monitorado pelo git usamos ------>  git add "nome do arquivo e a extensao sem aspas"</br>
ou git add"*.extensao" para adicionar tudo da extensao</br>
ou git add "." para adicionar toda a pasta</br>

git add -> passamos os arquivos para a area de espera, precisamos confirmar o projeto</br>

Comando:</br></br>
git commit -m "Teste1" -> salva mudanças e denifine um nome para o salvamento</br></br>
Para o git ignorar um arquivo -> criamos novo arquivo chamado".gitignore" e colocamos os arquivos lá</br></br>

git commit -a -m "Teste1" -> salva mudanças e pula etapa da area de espera</br></br>

-------------------------------------------------------------</br></br>
git diff -> Para consultar as alterações nos arquivos digitamos </br></br>
git diff --staged -> Consultar arquivos na area de espera</br></br>
git log -> mostra todos os commits feitos em nosso programa</br></br>
git log -p -> Mostra todas as linhas dos programas por paginação (Letra Q volta no terminal normal)</br></br>
git log -p (- "Especificar quantas linhas você deseja")</br></br>
git log --pretty=oneline -> Mostra o codigo e a mensagem de cada commit</br></br>
Interface Gráfica:</br></br>
gitk -> Para visualizarmos na interface grafica todas as alterações feitas</br></br>

-------------------------------------------------------------</br></br>
				Revertendo Situações:</br></br>

Para editar um commit:</br>
{  -> simbolico</br>
git add -> para adicionarmos o arquivo a ser editado</br>
git commit --ammend -m "nome da alteração" (edição - pode trocar o nome)</br>
}

git checkout -- (Nome do arquivo) -> Para restaurar um arquivo modificado</br>

Para remover arquivos:</br>
git rm (nome do arquivo)</br>
</br>
md -> cria nova pasta</br>

-------------------------------------------------------------</br>

				CRIANDO TAGS</br>

Uma tag ajuda a reverter, consultar arquivo antigo</br>

Criando -> git tag -a ("Nome da tag") -m ("Podemos incluir uma mensagem aqui")</br>
ex:</br>
git tag -a v1.0 -m "Versao 1.0"</br>

git tag -> mostra a versao que estamos, no caso nossa tag</br>
git show -> mostra os detalhes da tag que estamos ou se especificado a tag mostra detalhes da tag especificada</br>
git checkout -> faz a troca da tag pro ponteiro inicial, troca os arquivos</br>
git tag -d (nome da tag a ser deletada) -> deleta a tag</br>

-------------------------------------------------------------</br>
					BRANCH</br>
git branch (nome do branch) -> cria um branch</br>
git checkout teste -> transfere arquivos para o branch</br>

ou o comando</br>
git chechout -b (nome do branch) -> Realiza as duas linhas de cima de uma só vez</br>

Comitamos o branch pra implementar e utilizamos o comando -></br>
git merge (nome do branch)</br>

git branch -d (nome do branch) -> teleta branch de teste</br>

-------------------------------------------------------------</br>
					GITHUB</br>
ssh-keygen -> gera par de chaves ssh</br>
git clone (repositorio)-> clona repositorio (baixa ele pra maquina)</br>
git push origin master -> enviar arquivos pro repositorio</br>
git push -> transfere commits do repositório local a um repositório remoto</br>

-------------------------------------------------------------</br>

		Criando uma estação de trabalho pra um servidor</br>

git init --bare -> Para criar um repositorio dentro do servidor e nao da nossa maquina
Para o primeiro acesso do repositorio devemos clonar o repositorio 
 git clone file:////(nome do servidor sem os parenteses) "nome"</br>

git remote -> Para descobrir o nome do nosso repositorio remoto</br>
git push "nome" (brach)master -> Para enviar os arquivos para o repositorio </br>
git pull -> Pegar dados do servidor para a maquina </br>

