## Executar d
docker-compose up -d

## Fazer que o adonis se conecte com o banco de dados
npm install @adonisjs/lucid

## Configurar o banco depois de instalado orm
node ace configure @adonisjs/lucid

## Instalar pacote de autenticacao adonis
npm install @adonisjs/auth

## Configurar autenticacao adonis
node ace configure @adonisjs/auth

## criar uma validacao Rota - Validar se email e senha
node ace make:validator Auth/StoreValidator

## Criar controllers de Users
node ace make:controller Auth/Main -r

## Depois de feito o controller / routes e middleware rodar o migration
node ace migration:run

## criar tabela de chaves de autenticacao
node ace make:migration user_keys
