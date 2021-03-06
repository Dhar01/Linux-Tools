# Wildcards ðï¸

**Wildcards** (*also known as globbing*) allows us to select filenames based on patterns of characters.

| Wildcard | Meaning |
|----------|---------|
| `*` | matches any character |
| `?` | matches any single character |
| `[characters]` | matches any *character* that is a member of the *set characters* |
| `[!characters]` | matches any *character* that is <ins>not</ins> a member of the *set characters* |
| `[[:class:]]` | matches any *character* that is a member of the specified *class* |


ðâ Commonly used *character classes*:
| Character class | meaning |
|-----------------|---------|
| `[:alnum:]` | matches any alphanumeric character |
| `[:alpha:]` | matches any alphabetic character |
| `[:digit:]` | matches any numeral |
| `[:lower:]` | matches any lowercase letter |
| `[:upper:]` | matches any UPPERCASE letter |


#### Examples

`[[:upper:]]*` : Any file beginning with an uppercase letter.

`*[[:lower:]123]` : Any file ending with a lowercase letter or
the numerals â1â, â2â, or â3â.

`BACKUP.[0-9][0-9][0-9]` : Any file beginning with âBACKUP.â
followed by exactly three numerals.

`[abc]*` : Any file beginning with either an âaâ, a
âbâ, or a âcâ
