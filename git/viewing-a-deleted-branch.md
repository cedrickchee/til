# Viewing a Deleted File

I've deleted a file and then committed. The file is no longer in my working copy. I want to look at the contents of that file, but not actually restore it. I can do this:

```sh
$ git show HEAD^:path/to/file
```

You can use an explicit commit identifier or `HEAD~n` to see older versions or if there has been more than one commit since you deleted it.

```sh
$ git show HEAD~2:path/to/file
```

`path/to/file` is full path from the top of project (top directory of repository).

[source](https://stackoverflow.com/q/1395445/206570)
