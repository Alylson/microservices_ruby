# microservices_ruby

git clone https://github.com/Alylson/authentication_service
git clone https://github.com/Alylson/task_service
git clone https://github.com/Alylson/scraping_service
git clone https://github.com/Alylson/notification_service

docker-compose up -d --build

docker exec -it authentication_service rails db:create db:migrate
docker exec -it task_service rails db:create db:migrate
docker exec -it scraping_service rails db:create db:migrate
docker exec -it notification_service rails db:create db:migrate

