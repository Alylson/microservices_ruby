## Microserviços: Ruby On Rails

- Framework: Rails 7.1

## Versão do Ruby

- 3.3.1

## Versão do MySQL

- Utilizada versão 8.0

## 1 - Baixar os microserviços

Na raiz do projeto:
```
git clone https://github.com/Alylson/authentication_service
```

```
git clone https://github.com/Alylson/task_service
```

```
git clone https://github.com/Alylson/scraping_service
```

```
git clone https://github.com/Alylson/notification_service
```

## 2 - Build

Fazendo build da aplicação.

Na raiz do projeto:
```
$docker-compose up -d --build
```

## 3 - Rodar migration

```
docker exec -it authentication_service rails db:create db:migrate
```

```
docker exec -it task_service rails db:create db:migrate
```

```
docker exec -it scraping_service rails db:create db:migrate
```

```
docker exec -it notification_service rails db:create db:migrate
```

