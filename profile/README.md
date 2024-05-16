# enchentes-app-br

API de Geolocalização para Auxílios durante Enchentes no RS

## Proxy

Para desenvolvimento dos serviços, deve-se utilizar o proxy local que deve ser
inicializado com o comando abaixo.

```
git clone git@github.com:enchentes-app-br/proxy.git

docker compose \
    --project-directory ./proxy \
    up --detach
```
