V1:
docker build -t palashkosta/sampledocker -f DockerfileV1 .
docker run -p 8080:8080 palashkosta/sampledocker
docker exec -ti 3ab69504c7fd /bin/bash

V2:
mkdir target/dependency
cd target/dependency
jar -xf ../*.jar
docker build -t palashkosta/sampledocker:V2 -f DockerfileV2 .
docker run -p 8080:8080 palashkosta/sampledocker:V2
docker exec -ti ae49e7868ac5 /bin/bash

V3:
docker build -t palashkosta/sampledocker:V3 -f DockerfileV3 .
docker run -p 8080:8080 palashkosta/sampledocker:V3
docker exec -ti 4d0dda07a10f /bin/bash