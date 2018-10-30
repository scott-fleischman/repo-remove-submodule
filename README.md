# repo-remove-submodule

Test the GitHub API via the Haskell `github` library for repositories that have removed submodules.

In particular, a couple fields in the files array have null fields which are normally non-null:
```
"blob_url": null,
"raw_url": null,
```

See the [example response](github-api-response.json#L361) obtained by doing:

```sh
curl https://api.github.com/repos/scott-fleischman/repo-remove-submodule/compare/d03c152482169d809be9b1eab71dcf64d7405f76...42cfd732b20cd093534f246e630b309186eb485d
```
