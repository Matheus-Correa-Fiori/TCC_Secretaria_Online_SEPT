
# TCC - Secretaria Online do SEPT (Front-End)

Projeto desenvolvido em PHP para a interface da Secretaria, hospedado no repositório [TCC---Secretaria-UI](https://github.com/LucasPerussi/TCC---Secretaria-UI.git).

## 📋 Descrição

Este projeto fornece uma interface de usuário para a Secretaria, permitindo a gestão eficiente de diversas funcionalidades administrativas.

## 🚀 Tecnologias Utilizadas

- PHP
- Composer
- Bootstrap
- Javascript

## 🛠️ Instalação

Siga os passos abaixo para configurar o projeto localmente:

### 1. Clone o Repositório

```bash
git clone https://github.com/Matheus-Correa-Fiori/TCC_Secretaria_Online_SEPT.git
```

### 2. Extraia o arquivo .zip "TCC---Secretaria-Front.zip" e acesse o Diretório do Projeto

```bash
cd TCC---Secretaria-UI
```

### 3. Instale as Dependências com Composer

Certifique-se de ter o [Composer](https://getcomposer.org/) instalado em sua máquina. Em seguida, execute:

```bash
composer install
```

### 4. Configuração do Arquivo `Config.controller.php`

É necessário inserir o arquivo `Config.controller.php` no diretório `controller/`. Crie o arquivo `Config.controller.php` com o seguinte conteúdo:

```php
<?php
namespace API\Controller;

class Config
{
    // O IP local de sua máquina e substitua o nome da pasta criada
    const BASE_URL = "http://192.168.0.28/tcc-ui/";
    const DOMINIO = "/tcc-ui/";

    // Caso esteja usando a API localmente
    const API_URL = "localhost:3000/";


    const LOGIN_PAGE = self::BASE_URL . "login";
    const BASE_ACTION_URL = self::BASE_URL . "action";
    const BASE_CSS = self::BASE_URL . "src/css/";
    const BASE_JS = self::BASE_URL . "src/js/";
    const HOME_URL = self::BASE_URL . "dashboard";
    const BASE_PATH_JS = "src/js/";
    const SERVERNAME = "localhost";
}
```

**Passos para Configuração:**

1. **Crie o Arquivo:**

   Navegue até o diretório `controller/` e crie um novo arquivo chamado `Config.controller.php`.

2. **Adicione o Conteúdo:**

   Copie e cole o código acima no arquivo criado.

3. **Ajuste as Constantes:**

   - **BASE_URL:** Altere para o IP local da sua máquina onde o projeto será executado.
   - **API_URL:** Escolha entre usar a API local ou a online, comentando/descomentando conforme necessário.

## 🔧 Executando o Projeto

Após a configuração, você pode iniciar o servidor localmente. Apesar de recomendarmos o XAMPP, se estiver usando o PHP embutido, execute:

```bash
php -S localhost:8000
```

Acesse o projeto através do navegador em `http://localhost:8000`.

## 📞 Contato

Para mais informações, entre em contato através do [perussilucas@hotmail.com](mailto:perussilucas@hotmail.com).

---

# TCC - Secretaria Online do SEPT (API)

API responsável pelas funções lógicas da implementação da nova secretaria online do SEPT. Este projeto faz parte do trabalho de conclusão de curso da equipe de graduação em TADS na UFPR.

## 📋 Descrição

A API fornece os serviços necessários para gerenciar as funcionalidades da secretaria online, incluindo autenticação, gerenciamento de usuários e integração com o banco de dados.

## 🚀 Tecnologias Utilizadas

- Node.js
- TypeScript
- Express
- Prisma ORM
- JWT (Json Web Tokens)
- JEST (Testes)

## 🛠️ Instalação

Siga os passos abaixo para configurar o projeto localmente:

### 1. Clone o Repositório

```bash
git clone https://github.com/Matheus-Correa-Fiori/TCC_Secretaria_Online_SEPT.git
```

### 2. Extraia o arquivo .zip "TCC---Secretaria-API.zip" e acesse o Diretório do Projeto

```bash
cd TCC_Secretaria_Online_SEPT
```

### 3. Instale as Dependências

Certifique-se de ter o [Node.js](https://nodejs.org/) e o [npm](https://www.npmjs.com/) instalados. Em seguida, execute:

```bash
npm install
```

### 4. Configure o Arquivo `.env`

Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:

```
DATABASE_URL=mysql://root:@localhost:3306/tcc
DATABASE_URL_TESTS=mysql://root:@localhost:3306/tcc_tests
```

### 5. Configure o Banco de Dados

1. Crie os bancos de dados `tcc` e `tcc_tests` localmente.
2. Importe o script `tcc.sql`, localizado na pasta `db` do projeto, para ambos os bancos.

### 6. Inicie o Servidor

Para iniciar o servidor em desenvolvimento, execute:

```bash
npm run dev
```

Para rodar os testes, execute:

```bash
npm run test
```

**⚠️ Problemas ao iniciar o projeto?**  
Caso ocorra algum problema, rode os comandos abaixo e tente novamente:

```bash
npx prisma db pull
npx prisma generate
```

## 📖 Documentação Online

Você pode acessar a documentação da API em:

[https://documenter.getpostman.com/view/17286749/2sAY545dog](https://documenter.getpostman.com/view/17286749/2sAY545dog)

## 🔧 Scripts Disponíveis

- **Instalar dependências:**
  ```bash
  npm install
  ```

- **Iniciar servidor em desenvolvimento:**
  ```bash
  npm run dev
  ```

- **Iniciar servidor em produção:**
  ```bash
  npm start
  ```

- **Executar testes:**
  ```bash
  npm run test
  ```



## 📞 Contato

Para mais informações, entre em contato através do [perussilucas@hotmail.com](mailto:perussilucas@hotmail.com).

---
