---
layout: default
---
Learn all about ```GNU coreutils``` here: [https://www.gnu.org/software/coreutils/manual/coreutils.html](https://www.gnu.org/software/coreutils/manual/coreutils.html) 

# Common utils and their common usage:   
 
[numfmt](#numfmt)    
[tee](#tee)      
[wc](#wc)    


## <a name="numfmt">numfmt</a>
useful to convert integer from standard output to a floating point number or a string that can be used as a file name

```bash
$numfmt --format '%6f' 1
1

$numfmt --format '%06f' 1
000001

$numfmt --format '%10.6f' 1
  1.000000

$numfmt --format '%010.6f' 1
001.000000

$numfmt --format '%010.6f.txt' 1
001.000000.txt
```

                 
## <a name="wc">wc</a>

```bash
$wc -lwc file1 file2
```
gives  the number of lines, words, and characters in file1 and file2 as well as both files combined 

## <a name="tee">tee</a>
useful for redirecting standard output to a file

```bash
$./run.x  | tee outfile 
```

with ```-a``` option, the output will be appended instead of overwriting

```bash
$./run.x  | tee -a outfile 
```
