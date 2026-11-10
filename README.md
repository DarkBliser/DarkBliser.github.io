# Shelv invitation page

Messengers only make `https://` addresses clickable, so invitations to the Shelv app go through
`join/`. The page stores nothing and loads nothing from anywhere else.

The invitation's content comes after the `#` in the address. Browsers never send that part to a
server, so GitHub doesn't see it either.

`.well-known/assetlinks.json` tells Android that these links belong to the Shelv app, so tapping
one can open the app directly. It only contains the public fingerprints of the app's signatures: the Play key (25:A3…) and the
first key (11:5E…), which handed over to it.

`datenschutz/` is Shelv's privacy policy (German, then English). Google Play needs its address:
`https://darkbliser.github.io/datenschutz/`. Update its date when the content changes.
