# THECHAINDATA
This repo contains files and information for setting up your local env to work as a HTTPS address with a specific URL, to allow you to go from http:localhost to https:thechaindata.com

## Things that helped set this up:
https://www.freecodecamp.org/news/how-to-get-https-working-on-your-local-development-environment-in-5-minutes-7af615770eec/
https://www.youtube.com/watch?v=7isa-1VC6pY

## changing your /etc/hosts
go to: vim /etc/hosts
and add: 127.0.0.1    local.thechaindata.com

## helpful commands

### Compose up with an orphan check
docker-compose up -d --remove-orphan

### Checkout out the image by running it and sshing into it?
docker run -it --rm nginx:1.19-alpine sh

### Sometimes the container is still running but something has gone wrong and requests are getting 504 (Gateway timeout)
killall Docker && open /Applications/Docker.app

