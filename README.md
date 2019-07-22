# A simple dockerized SheepIt render farm client

Auto-updates the client on container startup.

There's probably a little more room for fat trimming, since this was adapted from an old Ubuntu VM setup script, but I'm satisfied with where things are currently.

## Instructions
Pretty similar to my old but fat one, just swap out your username and password.

```
docker run -d \
 --name "sheepit" \
 -e user_name=XXXXXX \
 -e user_password=XXXXXX \
 agsphoenix/sheepit-docker:latest
```

You can also specify the `cpu` variable to override autodetection; like `-e cpu=4`.

## Extra bits

[SheepIt client GitHub repo](https://github.com/laurent-clouet/sheepit-client)  
[SheepIt site](https://www.sheepit-renderfarm.com/)
