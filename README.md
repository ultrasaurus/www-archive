
## static copy of WordPress site

1. get web files
```
wget -r --trust-server-names www.ultrasaurus.com
```

2. absolute paths => relative paths:

```
find . -name '*' -exec sed -i -e 's/https:\/\/ultrasaurus\.com//g' {} \;

find . -name '*' -exec sed -i -e 's/https:\/\/www\.ultrasaurus\.com//g' {} \;
```

3. remove query args from filenames (rename css and js files in wp-includes director)

4. hide comments
```
.comments-link {display:none}
.comment-respond {display:none}
```
