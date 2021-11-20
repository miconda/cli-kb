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

## Control Core Dump File ##

Lift the core size limit:

```
ulimit -c unlimited
```

Enable core file per process:

```
echo "1" > /proc/sys/kernel/core_uses_pid
```

## SNGREP ##

Reading content from a live capture pcap file

```
tail -c +1 -f /tmp/sipdump.pcap | sngrep -I -
```

## GIT ##

Undo last commit without losing its changes:

```
git reset HEAD~1
```

Undo last commit and lose its changes:

```
git reset --hard HEAD~1
```

## OPENSSL ##

Generate random string with a specific length encoded base64:

```
openssl rand -base64 15
```

