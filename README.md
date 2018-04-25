# docker-angular-cli

Angular CLI Docker Image

## How to use

[Docker images sripad/angular-cli](https://hub.docker.com/r/sripad/angular-cli/)

docker pull sripad/angular-cli:node9.1.1-angular-cli-1.7.4

docker images

docker run -it --rm sripad/angular-cli:node9.1.1-angular-cli-1.7.4 node --version

docker run -it --rm sripad/angular-cli:node9.1.1-angular-cli-1.7.4 npm --version

docker run -it --rm sripad/angular-cli:node9.1.1-angular-cli-1.7.4 ng --version

## How Build/Push docker-angular-cli

eval "$(docker-machine env default)"

docker build -t node9-angular-cli-1.7.4 .

docker run -it --rm node9-angular-cli-1.7.4:latest

docker tag node9-angular-cli-1.7.4:latest sripad/angular-cli:node9.1.1-angular-cli-1.7.4

docker images

docker push sripad/angular-cli:node9.1.1-angular-cli-1.7.4
