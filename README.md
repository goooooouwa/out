RSS feeds of my favorite Posts & Podcasts generated by [blog_crawler](https://github.com/goooooouwa/blog_crawler/tree/master).

## What to do with these files?

### For podcasts, you can download mp3 files from file URLs with `mp3-urls.txt`

Run the following CURL download with a file with URLs to batch download files:

`xargs -n 1 curl -O -L --retry 5 --retry-max-time 60 -C - < ./mp3-urls-unique-id-fix.txt`

Explanation of CURL command:

- -O: download file
- -L: follow redirects
- --retry: retry x times
- --retry-max-time: retry x seconds at most

### For blogs, You can generate Kindle ebook from RSS feeds with `feeds.txt` and `slice-0.xml`

See [README](https://github.com/goooooouwa/blog2kindle/blob/master/README.md) of [blog2kindle](https://github.com/goooooouwa/blog2kindle/tree/master).
