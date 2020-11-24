# When using filters, certain characters must be escaped

| **Character** | **Escaped As** | **Note**                                      |
| -------|-----|------|
| “ | `” |Only needed if the data is enclosed in double-quotes.|
|‘ 	| \’ |Only needed if the data is enclosed in single quotes.|
|NUL|	\00|Standard LDAP escape sequence.|
|\ |\5c |Standard LDAP escape sequence.|
|* | \2a|Escaped automatically, but only in -eq and -ne comparisons. Use -like and -notlike operators for wildcard comparison.|
|( |/28 |Escaped automatically.|
|) |/29 |Escaped automatically.|
|/ |/2f |Escaped automatically.|
