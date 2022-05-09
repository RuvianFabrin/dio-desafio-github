

- Windows
	- cd //entra na pasta
	- dir //ver diretório
	- mkdir //criar pasta
	- del/rmdir //apagar pasta
	- echo hello > hello.txt //Cria arquivo
	- del workspace //Deleta os arquivos dentro da pasta
	- rmdir workspace /S /Q //Deleta a pasta com os arquivos dentro

- Unix
	- cd //Entra na pasta
	- ls //ver diretório
	- mkdir //criar diretório
	- rm -rf //deleta
	- echo hello > hello.txt //Cria arquivo
	- rm -rf workspace //deleta a pasta


No windos da pra habilitar o subsistem linux, para rodar comandos linux no windows.

- Objetos do GIT
	- blobs
	- trees - Armazena blobs ou outras trees
	- commits - Aponta para, tree, parente, autor, mensagem, timestamp


#### Chave SSH
Imagem>Settingd>SSH and GPG keys> SSH Keys

- No Git Bash > 
	- ssh-keygen -t ed25519 -C seuEmail 
	- ed25519 é o nome da criptografia
	- coloque a senha
	- cat nome_criptografia
	- Copie e cole no git hub
	- no cli
	- eval $(ssh-agent -s)
	- copie p pid
	- ssh-add coloque_a_chave_privada 
	- (exemplo:id_ed25519)
	- aí é só clonar por SSH


Inicia o Git
git Init

git config --global user.email "seuEmail"
git config --global user.name "Seu nome"

Para fazer o commit
git add *
git commit -m "Seu commit"

Mostra o status do arquivo
git status

move arquivos
mv arquivo.md ./

Untracked, Unmodified, modified, staged

Working Directory (git add)>staging area (git commit -m)>local repository

lista de suas configurações
git config --list

Caso name e email esteja diferente do github basta sobreescrever com o global

git config --global --unset user.email
git config --global --unset user.name

git config --global user.email "seuEmail"
git config --global user.name "Seu nome"


#### Para subir para o git hub
origin: é apenas um apelido
git remote add origin linkHTTPS

git remote -v
git push origin master
master é a branch do github


#### Resolvendo conflitos
Quando no github está mais novo que na sua máquina

no bash
git pull origin master

Aí abra os arquivos e ajuste oque deve ser juntado

git add *
git commit -m "Ajustado"
git push origin master

#### Pegando repositório
git clone caminho_https



