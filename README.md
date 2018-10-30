# repo-remove-submodule

Test the GitHub API via the Haskell `github` library for repositories that have removed submodules.

In particular, a couple fields in the files array have null fields which are normally not-null:
```
"blob_url": null,
"raw_url": null,
```
