Create an Angular project
# npm install -g angular-cli
# ng init
#===========================
1) Check the docker images:
# docker images

2) Remove docker image:
# docker rmi -f xxx
(rmi = remove image, -f = forece, xxx = 3 first charactors)

3) Check docker images are running
# docker ps

4) Build docker image
# docker build -t {ImageName}:{TagName} .
(-t = tag, let docker know build image with tagName)

5) Run docker image
# docker run -d --name {container_name} -p {host-port:exposed-port}  {image-name}

6) Stop docker image
# docker stop {container_name}

7) Pull mongo image from docker-hub
# docker pull mongo:lates

8) Build Docker-Compose
# docker-compose up --build

9) If build docker-compose with some error: No suc image: sha256
# docker-compose down

10) Delete all images
# docker rmi $(docker images -q)

11) Delete all containers
# docker rm $(docker ps -a -q)

12) Export docker image:
# docker image save {image} > {filePath.tar}

13) Import docker image
# docker image load < {filePath.tar}
