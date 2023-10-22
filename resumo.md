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

| COMANDO             | O que faz                              | Exemplo                       | Observações                                   |
| ------------------- | -------------------------------------- | ----------------------------- | ----------------------------------------------- |
| git init            | Cria um repositório                   |                               | Cria uma pasta .git oculta                      |
| git add             | Manda um arquivo para o stage          | git add site.html             | git add . = Adiciona todos os arquivos da pasta |
| git commit          | Manda um arquivo do stage para o .git  | git commit -m "mensagem"""    |                                                 |
| git status          | Retorna o status atual do repositório |                               |                                                 |
| git log             | Mostra o histórico de alterações    |                               |                                                 |
| git checkout        | Volta para uma versão antiga          | git checkout ee644a           | Só precisa dos 6 primeiros digitos             |
| git checkout master | Volta para a última versão           |                               |                                                 |
| git branch          | Cria um novo ramo                      | git branch pagina-de-servicos |                                                 |

Pasta (Projeto) -> Stage -> .git

Antes de enviar o arquivo de fato pelo repositório, devemos enviá-lo para o stage através do comando git add. Só depois disso que devemos utilizar o git commit para mandar de fato para a pasta .git

### 4 - Configurando o usuário no git

git config --global user.name Nome

git config --global user.email guilhermealves@id.uff.br
