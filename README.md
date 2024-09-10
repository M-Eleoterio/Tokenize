# Tokenize

Tokenize é um site ficcional de geração e organização de tokens de API. As funcionalidades foram desenvolvidas em 4 horas, baseadas em um teste da EuroSkills 2023.

## Rodando localmente: Pré-requisitos

- PHP (versão 7.4 ou superior)
- Composer

## Rodando localmente

1. Clone o repositório
   ```bash
   git clone https://github.com/usuario/tokenize.git

   ```
2. Navegue até o diretório do projeto
 ```bash
   cd Tokenize
  ```
3. Instale as dependências:
  ```bash
  composer install
  ```
4. Copie o arquivo `.env.example` pra `.env`:
```bash
  cp .env.example .env
```
5. Gere a chave:
  ```bash
  php artisan key:generate
  ```
6. Crie o banco SQLite, caso inexistente:
```bash
touch database/database.sqlite
```

7. Rode as migrations do banco de dados:
  ```bash
  php artisan migrate
  ```
8. Popule o banco de dados:
```bash
   php artisan db:seed
```
9. Inicie o servidor:
  ```bash
  php artisan serve
  ```
  O backend estará rodando em `http://localhost:8000`.

  ### Funcionalidades
  - Geração de tokens de APi únicos
  - Organização dos tokens via Workspaces

  ### Tecnologias
  - Laravel
  - PHP
  - Blade
  - SQL
