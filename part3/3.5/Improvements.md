# Improving kurkkumopo

## Before optimization

Program is ran as root making it insecure and image sizes are:

* ml-kurkkumopo-backend: 878MB
* ml-kurkkumopo-frontend: 952MB
* ml-kurkkumopo-training: 925MB

## After optimization

After fixes apps are not ran as root and sizes are:

* ml-kurkkumopo-backend: 879MB
* ml-kurkkumopo-frontend: 562MB
* ml-kurkkumopo-training: 925MB

Changing frontend to run on alpine almost halves the size however since backend and trainig requred multiple heavy libraries they couldn't be optimized simply. Running backend and training on alpine linux failed with my attempts even with requirements surpassing the original size. Sizes could be further improved by running docker-slim.