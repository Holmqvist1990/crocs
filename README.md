# crocs!

DOA; turns out there's a little something called [Crystalline](https://github.com/elbywan/crystalline)!
<br>
This is why you search before you implement...

## Usage

Install:
```
$ make install
crystal build --release src/main.cr
sudo mv main /usr/bin/ crocs
[sudo] password for user:
Installed crocs OK.
```

Help:
```
$ crocs -h
crocs!
    -v, --version                    Show version
    -h, --help                       Show help
    -n NAME, --namespace NAME        Namespace to search in
    -m NAME, --method NAME           Method to search for
    -l, --list                       List cache entries
    -a, --add                        Add an entry to the cache
    -c, --clear                      Clear the cache

Namespace and method can also be passed as args: './crocs string rind'
Method can be omitted to list all instance methods.
```

Searching:
```
$ crocs string rind
#rindex(search : Char, offset = size - 1)
  Returns the index of the last appearance of search in the string, If offset is present, it defines the position to end the search (characters beyond this point are ignored).

#rindex(search : String, offset = size - search.size) : Int32 | Nil
  Returns the index of the last appearance of search in the string, If offset is present, it defines the position to end the search (characters beyond this point are ignored).

#rindex(search : Regex, offset = size) : Int32 | Nil
  Returns the index of the last appearance of search in the string, If offset is present, it defines the position to end the search (characters beyond this point are ignored).

#rindex!(search : Regex, offset = size) : Int32
  Returns the index of the last appearance of search in the string, If offset is present, it defines the position to end the search (characters beyond this point are ignored).

#rindex!(search : String, offset = size - search.size) : Int32
  Returns the index of the last appearance of search in the string, If offset is present, it defines the position to end the search (characters beyond this point are ignored).

#rindex!(search : Char, offset = size - 1) : Int32
  Returns the index of the last appearance of search in the string, If offset is present, it defines the position to end the search (characters beyond this point are ignored).
```
