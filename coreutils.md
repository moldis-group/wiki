---
layout: default
---
Learn all about ```GNU coreutils``` here: [https://www.gnu.org/software/coreutils/manual/coreutils.html](https://www.gnu.org/software/coreutils/manual/coreutils.html) 

# Common utils and their common usage:   

[tee](#tee)     
[wc](#wc)    

                 
## <a name="wc">wc</a>

```bash
wc -lwc file1 file2
```
gives  the number of lines, words, and characters in file1 and file2 as well as both files combined 

## <a name="tee">tee</a>
useful for redirecting standard output to a file

```bash
./run.x  | tee outfile 
```

with ```-a``` option, the output will be appended instead of overwriting

```bash
./run.x  | tee -a outfile 
```
