# API de Chat WebSocket com Laravel

Este projeto é uma API de chat simples implementada com Laravel e WebSockets.

## Descrição

Esta API permite aos usuários enviar e receber mensagens em tempo real utilizando WebSockets. É uma implementação básica destinada a servir como ponto de partida para aplicações de chat mais complexas.

## Instalação

Clone o repositório e instale as dependências.

```bash
git clone [URL_DO_SEU_REPOSITORIO]
cd [NOME_DO_SEU_REPOSITORIO]
composer install
```
Configure o ambiente copiando o arquivo .env.example para .env e gerando uma chave para a aplicação.
```bash
cp .env.example .env
php artisan key:generate
```
Inicie o servidor de desenvolvimento.
```bash
php artisan serve
```
## Uso
Para enviar mensagens, utilize o endpoint POST /api/messages com os parâmetros message e username.
```bash
curl -X POST -H "Content-Type: application/json" -d '{"message": "Olá, mundo!", "username": "usuario"}' http://localhost:8000/api/messages
```

## Contribuição
Se você encontrou um bug ou quer contribuir com novas funcionalidades, sinta-se à vontade para criar um Issue.

## Licença

MIT License
