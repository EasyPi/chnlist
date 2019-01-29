ccplist
=======

```bash
curl -s https://raw.githubusercontent.com/felixonmars/dnsmasq-china-list/master/accelerated-domains.china.conf |
  cut -d/ -f2 |
    sed 's@^@||@' |
      base64 > ccplist.txt
```
