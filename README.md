# TCP Server message

## Message format

    | 2 bytes | x  bytes |
    | content length | content|

## Example

- msg1: [00 02 41 42] => content length 2, content "AB"    
- msg2: [00 03 41 42 41] => content length 3, content "ABA"

## Client Tag

Message tag is contents prefix:

```
length 10, content "#1#some"
```
