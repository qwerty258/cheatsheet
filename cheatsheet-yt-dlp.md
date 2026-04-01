yt-dlp
======

```sh
# get list of resources
yt-dlp --js-runtimes node --proxy socks5://proxy.local:1080 -F URL
# get specific resource
yt-dlp --js-runtimes node --proxy socks5://proxy.local:1080 -o "%(uploader)s-%(upload_date)s-[%(id)s]-%(title)s.%(ext)s" -f 1 URL
# get list info
yt-dlp --js-runtimes node --proxy socks5://proxy.local:1080 --skip-download --flat-playlist --print "%(uploader)s-%(upload_date)s-[%(id)s]-%(title)s" URL
```
