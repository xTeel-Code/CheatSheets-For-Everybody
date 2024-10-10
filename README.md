# CheatSheets-For-Everybody

## Operators
Bash Code
```bash
#!/bin/bash
# Count number of characters in a variable:
#     echo $variable | wc -c

# Variable to encode
var="nef892na9s1p9asn2aJs71nIsm"

for counter in {1..35}; do
  var=$(echo $var | base64)
  if [[ counter -eq 35 ]]; then
    echo $var | wc -c
  fi
done
```
---
IF Operators
| Operator | Description        |
|---------|-------------------|
| -eq  | equal to             |
| -lt     | less than         |
| -le | less than or equal to |
|-eq |	is equal to           |
-ne |	is not equal to       |
-gt |	is greater than       |
-ge |is greater than or equal to |
---
File Operators
| Operator | Description                                                   |
|----------|---------------------------------------------------------------|
| -e       | if the file exists                                             |
| -f       | tests if it is a file                                          |
| -d       | tests if it is a directory                                     |
| -L       | tests if it is a symbolic link                                 |
| -N       | checks if the file was modified after it was last read         |
| -O       | if the current user owns the file                              |
| -G       | if the file’s group id matches the current user’s              |
| -s       | tests if the file has a size greater than 0                    |
| -r       | tests if the file has read permission                          |
| -w       | tests if the file has write permission                         |
| -x       | tests if the file has execute permission                       |

