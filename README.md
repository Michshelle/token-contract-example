# Simple token contract


## Updated based on the original repo
code is modified due to below changes:

ligo upgraded

taquito upgraded

## Special Usage
run `npm install`, `npm run build` and `node cli.js deploy 500 (or whatever amount here, no need to be 500)`.

You should see the KT1 has been created.  After that,

modify the build.js, remove the output to be json, and modify the storage to be Token.ml.

run again `npm run build`, now you should get Token.ml under contract folder.


run under tezos folder: `./tezos-client get script entrypoints for Token.ml` to check up the entrypoint and input format.

After that, you can do something according to the output, like `./tezos-client transfer 0 from blublublue to KT1SmPNJAsJH4p3bxZ1cHNWj66RkEk5e1j9V --entrypoint approve --arg '(Pair "tz1McNt8ByDbhV5BVbc9Cx49suvjcGva56yF" 12)' --burn-cap 1`


# BELOW IS FROM ORIGINAL README#######################

## Install

Run `npm install`

Run `npm run build`

## Using the cli for example

`node cli.js deploy 200`

`node cli.js storage KT1Kz1kXu39VKTpcAY1M3BWuv4zGp55i9Zsy`

`node cli.js bigMap KT1Kz1kXu39VKTpcAY1M3BWuv4zGp55i9Zsy tz1bwsEWCwSEXdRvnJxvegQZKeX5dj6oKEys`


