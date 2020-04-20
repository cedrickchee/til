# Write Out an HTML File with Cover Tool

`go tool cover-html=coverage.out` appears to use `xdg-open` on Linux, which doesn't always select the right browser. Even if the `$BROWSER` environment variable is set, the cover tool doesn't always select the right browser. In some cases, the browser window doesn't pops up at all.

You can use the flag `-o` to write out an HTML file instead of launching a web browser and then use the web browser to open the file.

```sh
$ go tool cover -html=c.out -o coverage.html
```

[source](https://github.com/golang/go/issues/10365#issuecomment-93143893)
