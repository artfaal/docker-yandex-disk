# docker-yandex-disk


Container with Ya.Disk inside

How to run:

```
docker run -d -it --name yadisk \
 -e YANDEX_USER=<login> \
 -e YANDEX_PASSWORD=<password> \
 --restart=always \
 artfaal/docker-yandex-disk
 ```


Now you can mount files from another container with `--volumes-from yadisk`


Files would be available in `/var/lib/selenium` folder.
