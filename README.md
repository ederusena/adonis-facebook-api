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
