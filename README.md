# Bash Explorer
This bash utility is intended to make the inspection of entities within the filesystem by detecting the type of a file system object and then executing the most reasonable command to find out more about it. In the case of text files, this means displaying the contents with less. In all other cases, the object is inspected with ls.

Two flags are availble. 
* `-v` puts `explorer` in verbose mode and all calls to `ls` will include `-la` flags.
* `-e` will cause `explorer` to edit any text file it encounters using the editor specified in the `EDITOR` environment variable. If you have not set `EDITOR`, explorer will quit.
