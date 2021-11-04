# I-am-lazy-so-I-keep-my-linux-commands
Some commands that I use repeatedly

* count files recursively
```shell
find <src> -type f | wc -l
```


* copy certain files/types of files while also keep the directory structure (copy all jpg files in the example, \; means ending the command)
```shell
find <src> -name '*.jpg' -exec cp --parents \{\} <dst> \;
```


* delete all empty subdirectories and print them, thry this without -delete to check first!!!
```shell
find <src> -type d -empty -print -delete
```

