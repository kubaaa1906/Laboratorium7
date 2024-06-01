# Laboratorium7

1. Polecenie do stworzenia buildera: docker buildx create --name lab7builder --driver docker-container --bootstrap
2. Polecenie do ustawienia stworzonego buildera jako domyślny: docker buildx use lab7builder
3. Polecenie do budowy obrazu: docker buildx build -f Dockerfile3 -t docker.io/kubaa1906/laboratorium7:lab7 --platform       linux/amd64,linux/arm64 --push --cache-to=type=registry,ref=kubaa1906/laboratorium7:cache,mode=max --cache-from=type=registry,ref=kubaa1906/laboratorium7:cache .

Link do DockerHub: https://hub.docker.com/repository/docker/kubaa1906/laboratorium7/general
