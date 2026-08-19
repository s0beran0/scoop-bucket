# scoop-bucket

Scoop bucket for [`ngx`](https://github.com/s0beran0/ngx), a CLI that makes
nginx readable by a program.

```powershell
scoop bucket add s0beran0 https://github.com/s0beran0/scoop-bucket
scoop install ngx
```

## What is here

`ngx.json`, written by the `ngx` release workflow. Nothing in this repository
is edited by hand: every `vX.Y.Z` tag on `s0beran0/ngx` regenerates the
manifest and pushes it here.

## Updating

`ngx` installed this way does not update itself. It knows it came from Scoop —
`ngx version` reports `install_channel` — and `ngx update` refuses, pointing at
the command that does the job properly:

```powershell
scoop update ngx
```

Replacing a file Scoop believes it owns would leave its database describing
something that is no longer there.
