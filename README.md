# Blog do Bill

Um aplicativo de blog simples desenvolvido com PHP e o framework Laravel. Este projeto permite criar, visualizar e gerenciar postagens de blog categorizadas por temas como Tecnologia, Laravel, PHP e JavaScript.

## Funcionalidades
- Criar e exibir postagens de blog com títulos, slugs, conteúdo, trechos e categorias.
- Categorizar postagens (ex.: Tecnologia, Laravel, PHP, JavaScript).
- Filtrar postagens publicadas e ordenar por data de criação mais recente.
- Gerenciamento básico de sessões usando o driver de banco de dados.

## Requisitos
- PHP 8.2 ou superior
- Composer
- MySQL
- Laravel 12.x
- XAMPP (para desenvolvimento local com Apache e MySQL)

## Instalação

### 1. Clone o Repositório
```bash
git clone https://github.com/seu-usuario/blog-do-bill.git
cd blog-do-bill
```

### 2. Instale as Dependências
Certifique-se de que o Composer está instalado, então execute:
```bash
composer install
```

### 3. Configure o Ambiente
- Copie o arquivo `.env.example` para `.env`:
  ```bash
  copy .env.example .env
  ```
  (No Windows, use `copy` em vez de `cp`.)
- Edite o arquivo `.env` com as suas configurações de banco de dados:
  ```
  DB_CONNECTION=mysql
  DB_HOST=127.0.0.1
  DB_PORT=3306
  DB_DATABASE=bd_blog_do_bil
  DB_USERNAME=seu_usuario
  DB_PASSWORD=sua_senha
  ```
- Gere uma chave de aplicativo:
  ```bash
  php artisan key:generate
  ```

### 4. Configure o Banco de Dados
- Crie o banco de dados `bd_blog_do_bil` no MySQL (via phpMyAdmin ou linha de comando).
- Execute as migrações para criar as tabelas necessárias:
  ```bash
  php artisan migrate
  ```

### 5. Inicie o Servidor
- Use o Artisan para iniciar o servidor de desenvolvimento:
  ```bash
  php artisan serve
  ```
- Acesse o blog em `http://127.0.0.1:8000` no seu navegador.

## Uso
- **Página Inicial**: Visualize todas as postagens publicadas em `http://127.0.0.1:8000/posts`.
- **Detalhes da Postagem**: Acesse uma postagem específica usando seu slug, por exemplo, `http://127.0.0.1:8000/posts/tecnologia`.
- Adicione novas postagens ou categorias através do código ou de um painel administrativo (se implementado).

## Contribuição
Sinta-se à vontade para contribuir! Envie pull requests ou abra issues no repositório.

## Licença
Este projeto é de código aberto sob a [licença MIT](LICENSE) (ou especifique sua licença preferida).

## Data de Criação
09/06/2025, 21:00 -03
