The following regex is one of the options that can be used:
```
/(\S{2,})\1/
```
We are capturing more than two non-whitespace characters which are repeated two times. The `{2,}` does not capture the two `s` of `impossible` for example.

We need to substituite all matched text with the capture group that we created:
```
s/(\S{2,})\1/\1/g
```
