# Resumo de Git e Github

### 1 - Teoria

Git -> É o versionamento de código. Ou seja, criamos várias versões de um projeto.

Repositório ->

Branch -> Cria uma nova linha do tempo

Merge -> Junta todas as modificações. Útil quando temos vários programadores e queremos juntar as modificações de todos.

Github -> Serve para hospedar repositórios.

### 2 - Testando se o git está instalado

1. Abra o terminal de comando
2. git --version (Se retornar alguma versão é porque está instalado)

### 3 - Comandos

| COMANDO                        | O que faz                                | Exemplo                                   | Observações                                                     |
| ------------------------------ | ---------------------------------------- | ----------------------------------------- | ----------------------------------------------------------------- |
| git init                       | Cria um repositório                     |                                           | Cria uma pasta .git oculta                                        |
| git add                        | Manda um arquivo para o stage            | git add site.html                         | git add . = Adiciona todos os arquivos da pasta                   |
| git commit                     | Manda um arquivo do stage para o .git    | git commit -m "mensagem"""                |                                                                   |
| git status                     | Retorna o status atual do repositório   |                                           |                                                                   |
| git log                        | Mostra o histórico de alterações      |                                           | Para sair do git log, aperte a tecla q                            |
| git checkout                   | Muda de commits                          | git checkout ee644a                       | Só precisa dos 6 primeiros digitos                               |
| git checkout master            | Volta para a última versão             |                                           |                                                                   |
| git branch                     | Cria um novo ramo                        | git branch pagina-de-servicos             |                                                                   |
| git merge                      | Junta branchs                            | git merge pagina-de-servico               |                                                                   |
| git clone                      | Clona um repositório                    | git clone url                             |                                                                   |
| git pull origin                | Atualiza o repositório                  |                                           | Sempre faça antes de fazer o merge e quando começar a trabalhar |
| git push origin nome-do-branch | Mandando as atualizações para o github | git push origin nova-imagem-na-pg-servico |                                                                   |
| git branch -m novo-nome        | Muda o nome de um branch                 | git branch -m main                        |                                                                   |

Pasta (Projeto) -> Stage -> .git

Antes de enviar o arquivo de fato pelo repositório, devemos enviá-lo para o stage através do comando git add. Só depois disso que devemos utilizar o git commit para mandar de fato para a pasta .git

### 4 - Configurando o usuário no git

git config --global user.name Nome

git config --global user.email guilhermealves@id.uff.br

### 5 - Arquivo .gitignore

Serve para o git ignorar alguns arquivos

Crie um arquivo chamado .gitignore e coloque dentro dele linha por linha os arquivos e extensões que deseja ignorar.

Exemplo:

node_modules
index.txt
*.obj
*.cs

ignora a pasta node_modules, index.txt e todos os arquivos com extensão .obj e .cs

## 6 - Github

Criando um novo repositório e linkando ao seu projeto.

    1) Abra o seu perfil no github
	2) Clique no símbolo de + para criar um novo repositório
	3) New repository
	4) Nomeie e descreva o seu repositório e depois crie
	5) Insira os comandos sugeridos na página no terminal

Persistindo alterações no repositório remoto
	git push origin nome-do-branch
	git push origin nova-imagem-na-pg-servicos

FORK
	Criar uma cópia de algum repositório só para mim
