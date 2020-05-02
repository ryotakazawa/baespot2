*To start*
git clone https://github.com/ryotakazawa/baespot2.git

docker-compose build

docker-compose run -u root backend bundle

docker-compose run frontend yarn

docker-compose up

docker-compose exec backend bin/rails db:create

docker-compose exec backend bin/rails db:migrate

docker-compose exec backend bin/rails db:seed
