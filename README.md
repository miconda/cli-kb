# Command Line Knowledge Base #

Commands used not that often to remember by heart, but useful to collect and save time searching
the web to figure out them again in the future.

## IPv4 Convertion ##

### Integer Representation To String ###

```
echo -e "import ipaddress\nprint(ipaddress.IPv4Address(167772161))" | python3
```

Shows:

```
10.0.0.1
```

### String Representation To Integer ###

```
echo -e "import ipaddress\nprint(int(ipaddress.IPv4Address('10.0.0.1')))" | python3
```

Shows:

```
167772161
```
