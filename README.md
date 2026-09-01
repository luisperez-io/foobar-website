# foobar-website
[FooBar-io](https://foobar-io.net) Container configuration and content (md files to be rendered by [Hugo](https://gohugo.io))

## notes
The following commands needed to be run for the Hugo initialization files to be created and populated.

```{bash}
  docker run --rm -it \\n  -v "$PWD:/src" \\n  -w /src \\n  hugomods/hugo:exts \\n  mod init github.com/luisperez-io/foobar-website
  docker run --rm -it \\n  -v "$PWD:/src" \\n  -w /src \\n  hugomods/hugo:exts \\n  mod get github.com/adityatelange/hugo-PaperMod
```

- `go.mod` declares project’s Go/module dependencies.
- `go.sum` records cryptographic checksums verifying the exact dependency versions downloaded.

The commands only need to be run again if a change or update in the PaperMod version or another Hugo module dependency is done.
