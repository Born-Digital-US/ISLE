```
apt-get update && apt-get install -y emacs iputils-ping
chown -R islandora:www-data /var/cache/apache2/mod_cache_disk

a2enmod cache_disk
curl -O http://www.loc.gov/standards/mods/xml.xsd
curl -LsD - -o /dev/null http://www.loc.gov/standards/mods/xml.xsd
```

next to do:
- use traefik to route www.loc.gov through apache container
- `echo "TEST 123 TEST 123" >> /var/cache/apache2/mod_cache_disk/Fr/m6/gz8YIqKWS_tQjfBGgw.header.vary/HM/wl/M1FJKOuWg0YokaKfCA.data`
