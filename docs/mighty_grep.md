# 📌 grep

`grep`: **G**lobal **R**egular **E**xpression **p**rint.

`grep` is a powerful program used to find text patterns within files. It uses **regular expressions** (*shortly regex*) to match the pattern. 

When `grep` encounters a *pattern* in the file, it prints out the lines containing it. 

If no file is given, it will recursively search the given pattern in the files of current directory.

> `grep` is case-sensitive.

```bash
grep pattern [file...]

$ grep -n <search-pattern> file.txt
```

- `-n` : To show the line number in the output.

- `-i`: To ignore case-sensitive.

- `-v` : To print only those lines that do not match the pattern.
  
  

Use some special characters or regular expressions in grep:

- `^` : search at the beginning of the line.
- `$` : search at the end of the line.
- `.` : search any character.

## Variants

grep has two variants:

1. **egrep** : Extended grep.
2. **fgrep** : fast grep.

### egrep

`egrep` allows to use complicated regex.

For example, search any words that start with either `I` or `o`:

```bash
egrep '^(i/o)' file.txt
```

search any words starts in the range between `i` to `u`:

```bash
egrep '^[i-u]' file.txt
```

# fgrep
