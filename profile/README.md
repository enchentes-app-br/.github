# enchentes-app-br

API de Geolocalização para Auxílios durante Enchentes no RS

## Proxy

Para desenvolvimento dos serviços, deve-se utilizar o Proxy local que deve ser
inicializado com os comandos abaixo.

```console
git clone git@github.com:enchentes-app-br/proxy.git

docker compose \
    --project-directory ./proxy \
    up --detach
```

## Exemplo

Cada serviço possui o seu próprio repositório. Por exemplo, para trabalhar com o
serviço de Tokens e Donations, deve-se executar os seguintes comandos:

```console
git clone git@github.com:enchentes-app-br/tokens.git

docker compose \
    --project-directory ./tokens \
    run --rm install

docker compose \
    --project-directory ./tokens \
    up --detach
```

```console
git clone git@github.com:enchentes-app-br/donations.git

docker compose \
    --project-directory ./donations \
    run --rm install

docker compose \
    --project-directory ./donations \
    up --detach
```
