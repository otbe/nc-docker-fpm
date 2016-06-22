# nextcloud fpm docker image
This is a port from the awesome fpm docker image from [here](https://hub.docker.com/_/owncloud/).

## Migrating
If you would like to migrate from owncloud to nextcloud and you are an user of the original ```9.0.2-fpm``` image, just replace
it by this image. :)

## Example
Additionally there is a small example which bootstraps a _nginx + nextcloud + redis + mysql_ multi-container setup via ```docker-compose```.

Just run
```
$ cd example
$ docker-compose up
```

```nextcloud``` should be available at ```http://localhost```.

_Note:_ DB name and password (for root user) is only once needed to be set as environment variable.
After the initial start of the mysql container it can be removed from the compose file.