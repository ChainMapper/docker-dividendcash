# docker-dividendcash
Wallet and daemon for Dividend Cash [DVD] cryptocurrency on docker

# Quickstart
Type `docker run -it -e "USER=me" -e "PASSWORD=secret" -e "RPCALLOW=127.0.0.1" chainmapper/dividendcash` and see the wallet starting.

Alternatively type `docker run -it -v "<path_to_config>:/config/dividendcash.conf" chainmapper/dividendcash` to use your own config.

```
Docker DVD wallet

By: ChainMapper
Website: https://chainmapper.com

Starting DVD daemon...
```

# Proper start
Use a volume to store all data. The image stores it's data in `/data`. So mapping that volume will do the trick.

Additionally you can override the config and wallet file using volumes pointing to `/config/dividendcash.conf` and `/config/wallet.data`

# License
MIT, see LICENSE file