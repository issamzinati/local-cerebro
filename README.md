local-cerebro
-------------

You can setup the elasticsearch hosts from this [config file](./cerebro/config/app.conf). At line 83 you can find an example.
```
hosts = [
  {
   host = "http://host.docker.internal:59200"
   name = "prod cluster - main"
   headers-whitelist = [ "x-proxy-user", "x-proxy-roles", "X-Forwarded-For" ]
  }
]
``` 

### How to run ###
```
# To start cerebro
docker-compose up --build 

# To stop cerebro
docker-compose down
```