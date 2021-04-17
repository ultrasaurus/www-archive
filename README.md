


```
wget -r --trust-server-names www.ultrasaurus.com
```

absolute paths => relative paths:

```
find . -name '*' -exec sed -i -e 's/https:\/\/ultrasaurus\.com//g' {} \;

find . -name '*' -exec sed -i -e 's/https:\/\/www\.ultrasaurus\.com//g' {} \;
```