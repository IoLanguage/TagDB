# TagDB 
> DEPRECATED

Binding for <a href=http://www.dekorte.com/projects/opensource/tagdb/>tagdb</a> - a tagging database usefull for flickr-like tag searches.

Example use:
```Io
tdb := TagDB clone

tdb setPath("test")
tdb open

writeln("size = ", tdb size)
tdb atKeyPutTags("f430 for sale", list("red", "ferrari"))
tdb atKeyPutTags("lotus esprit", list("lotus", "esprit"))
writeln("size = ", tdb size)
keys := tdb keysForTags(list("lotus"))
writeln("keys = ", tdb symbolForId(keys at(0)))
tdb close
tdb delete
```

# Installation
`tagdb` should be installed and foundable in your system. Then:
```
eerie install https://github.com/IoLanguage/TagDB.git
```
