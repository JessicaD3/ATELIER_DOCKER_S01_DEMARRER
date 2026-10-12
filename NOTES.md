# Notes séance Docker

## Hello world + Apache
docker run hello-world
docker run -d -p 8080:80 --name mon-site httpd:2.4

## Tetris (Docker Hub)
docker run -d -p 8081:80 --name tetris bsord/tetris

## Serveur web avec volume
docker run -p 82:80 -v /tmp:/usr/local/apache2/htdocs/:ro -d quay.io/ocp-edge-qe/httpd
git clone https://github.com/bstocker/Maison_SVG.git
mv ./Maison_SVG/* /tmp
