# shared-services
## gitlab-CE
Перед запуском docker-compose необходимо создать докер сеть с соответствующим именем, либо задачть своё имя и поправить в файле docker-compose имя сети.
Например: docker network create \
  --driver=bridge \
  --subnet=172.28.5.0/27 \
  --ip-range=172.28.5.0/27 \
  --gateway=172.28.5.1 \
  my-network
