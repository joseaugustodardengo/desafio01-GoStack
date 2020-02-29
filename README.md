# Armazene tarefas
Projeto onde foi criado uma aplicação para armazenar projetos e suas tarefas

# Instalação
1) Necessário ter instalado na máquina o [Node](https://nodejs.org/en/) e um gerenciador de pacotes como [Yarn](https://yarnpkg.com/) ou [NPM](https://www.npmjs.com/).
2) Se você tem instalado o [Git](https://git-scm.com/) na máquina, pode clonar o repositório clicando em **Clone or download**.
3) Após ter feito a instalação necessária, poderá utilizar o projeto em um editor de sua preferência, mas recomendo o [VSCode](https://code.visualstudio.com/), pois já faz uma boa integração com as ferramentas que foram instaladas.
4) Recomendo utilizar a ferramenta [Insomnia](https://insomnia.rest/)

# Como usar
1) Abrir o terminal e realizar os seguintes comandos para instalar todas as dependências do projeto. Podendo ser o yarn ou npm, fica a seu critério
```
yarn ou npm install
```

## Como executar
No terminal executar os seguintes comandos e seu projeto já estará em execução.
```
yarn dev ou npm dev
```
Após, abrir o browser e colocar o seguinte caminho: **localhost:3000** e executar as tarefas de acordo com as informações do arquivo **index.js**
com as seguintes rotas:
```
http://localhost:3000/projects -          Listagem de projetos
http://localhost:3000/projects -          Criar um projeto
http://localhost:3000/projects/1/tasks -  Criar tarefa para projeto
http://localhost:3000/projects/1 -        Editar um projeto (altera somente título)
http://localhost:3000/projects/2 -        Deletar o projeto

```

### Exemplo de como criar um projeto dentro do Insomnia. 
É preciso fazer um JSON para inserir os dados dentro da rota **http://localhost:3000/projects** com o método POST.

```
{	
   "id": "1",
   "title": "Novo projeto 1",
   "tasks": []      
}
```

### Exemplo de como criar uma tarefa dentro projeto dentro do Insomnia. 
É preciso fazer um JSON para inserir os dados dentro da rota **http://localhost:3000/projects/1/tasks** com o método POST.
```
{	   
   "title": "Nova tarefa 1"   
}
```

# Tecnologias usadas
* [Node](https://nodejs.org/en/)
* [Yarn](https://yarnpkg.com/)
* [Express](https://expressjs.com/pt-br/)
