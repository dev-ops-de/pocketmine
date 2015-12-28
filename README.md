# pocketmine Docker image

## to run:
docker run -d -it -p 19132:19132/tcp -p 19132:19132/udp --name mcpe diceone/pocketmine:latest

## persistant data:
mkdir /srv/pocketmine
## run:
docker run -d -it -p 19132:19132/tcp -p 19132:19132/udp  -v /srv/pocketmine:/data --name mcpe diceone/pocketmine:latest

## for Administration:
docker attach mcpe
