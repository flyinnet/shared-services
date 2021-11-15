# shared-services
## gitlab-CE
Перед запуском docker-compose: 
1. необходимо создать докер сеть с соответствующим именем, либо задать своё имя и поправить в файле docker-compose имя сети.
Например: docker network create \
  --driver=bridge \
  --subnet=172.28.5.0/27 \
  --ip-range=172.28.5.0/27 \
  --gateway=172.28.5.1 \
  my-network
Для дополнительной информации иди по ссылке: https://docs.docker.com/engine/reference/commandline/network_create/
2. Необходимо задачть пароли в файлах docker-compose для postgres и в файле: ./containers/gitlab/gitlab_config/gitlab.rb
