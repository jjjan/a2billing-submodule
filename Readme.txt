do before any deployment
docker network create --driver=overlay proxy
docker stack deploy -c traefik.yml traefik

attention traefik is just for example

===========================================
cd /a2billing
docker-compose up -d