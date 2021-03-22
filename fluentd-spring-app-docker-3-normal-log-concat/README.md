* Projekt `demo` loguje standardnim Spring Boot zpusobem

cd demo

# Provede build image aplikace
mvnw spring-boot:build-image

cd ..

# Spusti elasticsearch, kibana, fluentd & aplikaci
docker-compose up --build

# Kibana:
http://localhost:5601

# Vsechno smazne:
docker-compose down
