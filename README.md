# XRPL Testnet Docker with XPOP

NetworkID: [ 1 ]

This container (run `./up`) spins up a docker container `xrpl-testnet` with XPOP exports enabled.

XPOP will be stored on B2M in the `xpop` directory.

To monitor state (`CTRL-C` to quit) run:

```bash
watch 'docker exec xrpl-testnet rippled --silent server_info|egrep "ledger|upti|peer"'
```

## B2M

Plays nice with this repo for Xahau testnet:
https://github.com/Xahau/Xahau-Testnet-Docker

And with this code for B2M:
https://gist.github.com/WietseWind/cd8a7a8c88f218fe7b768f59a665685d
