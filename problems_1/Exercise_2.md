The following regex is one of the options that can be used:
```
\(\S{2,})\1\
```
We are capturing more than two non-whitespace characters which are repeated two times. The `{2,}` does not capture the two `s` of `impossible` for example.
