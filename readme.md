V1: <br>
docker build -t palashkosta/sampledocker -f DockerfileV1 . <br>
docker run -p 8080:8080 palashkosta/sampledocker <br>
docker exec -ti 3ab69504c7fd /bin/bash <br>

V2: <br>
mkdir target/dependency <br>
cd target/dependency <br>
jar -xf ../*.jar <br>
docker build -t palashkosta/sampledocker:V2 -f DockerfileV2 . <br>
docker run -p 8080:8080 palashkosta/sampledocker:V2 <br>
docker exec -ti ae49e7868ac5 /bin/bash <br>

V3: <br>
docker build -t palashkosta/sampledocker:V3 -f DockerfileV3 . <br>
docker run -p 8080:8080 palashkosta/sampledocker:V3<br>
docker exec -ti 4d0dda07a10f /bin/bash <br>
