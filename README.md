# 🚀 **API Minhas Tarefas**

> O **frontend Minhas Tarefas** também foi desenvolvido e está disponível. Para conferir como ficou, [clique aqui](https://github.com/matheus-programmer/trabalho_final-front).

A **API Minhas Tarefas** fornece todas as funcionalidades principais para gerenciar uma lista de tarefas, incluindo a persistência das tarefas em um banco de dados. Este backend foi desenvolvido como parte do trabalho final da disciplina de **Desenvolvimento de Plataformas Web**.

## 🔧 Funcionalidades

A API oferece as seguintes operações para manipulação de tarefas:

- **Criação de usuário**  
  `[POST] /register`  
  Cria um novo usuário.

- **Autenticação de usuário**  
  `[POST] /login`  
  Autentica o usuário e gera um token JWT para acesso à API.

- **Listagem de tarefas**  
  `[GET] /tasks`  
  Retorna todas as tarefas do usuário autenticado.

- **Criação de tarefas**  
  `[POST] /task`  
  Cria uma nova tarefa para o usuário autenticado.

- **Remoção de tarefas**  
  `[DELETE] /task/:id`  
  Remove uma tarefa específica pelo seu ID.

- **Atualização de tarefas**  
  `[PUT] /task/:id`  
  Atualiza os dados de uma tarefa específica pelo seu ID.

## 🛠️ Tecnologias Utilizadas

A API foi construída utilizando as seguintes tecnologias:

- **Node.js** (v20.14.0)
- **Express** (framework web para Node.js)
- **MongoDB Atlas** (serviço de banco de dados MongoDB na nuvem)
- **Mongoose** (biblioteca ODM para MongoDB)

## 🏁 Como Executar o Projeto

### 1. **Certifique-se de que o Node.js está instalado**

Antes de iniciar, verifique se você possui o Node.js instalado em sua máquina. Se não tiver, [baixe e instale o Node.js](https://nodejs.org/).

### 2. **Clone o Repositório**

Clone o repositório do projeto para a sua máquina:

```bash
git clone <URL_DO_REPOSITORIO>
cd <nome_do_repositorio>
```

### 3. **Instale as Dependências**

Após clonar o repositório, instale as dependências do projeto:

```bash
npm install
```

### 4. **Configure o Arquivo `.env`**

Crie um arquivo `.env` na raiz do projeto. Você pode se basear no arquivo `.env.example` para configurar as variáveis necessárias. 

Exemplo de configuração para o arquivo `.env`:

```
MONGODB_URI="sua_url_de_conexao_com_o_mongodb"
PORT=3333
SECRET_KEY="minhachavesecreta"
```

- **MONGODB_URI**: Defina a URL de conexão com o seu banco de dados MongoDB (se estiver usando o MongoDB Atlas, você pode obtê-la na sua conta do Atlas).
- **PORT**: A porta na qual o servidor vai rodar (padrão é `3333`).
- **SECRET_KEY**: Uma chave secreta para criptografia e autenticação JWT. Escolha uma chave segura.

### 5. **Inicie o Servidor**

Com tudo configurado, inicie o servidor backend com o seguinte comando:

```bash
npm run dev
```

Se tudo estiver configurado corretamente, o backend estará rodando e você poderá interagir com a API.

---

## 📄 Conclusão

Agora a **API Minhas Tarefas** estará pronta para ser utilizada junto com o **frontend Minhas Tarefas**. Você pode começar a realizar operações de gerenciamento de tarefas, como autenticação de usuários e manipulação de tarefas via as rotas fornecidas.