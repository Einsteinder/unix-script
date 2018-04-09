# unix-script

## wikistats

The Wikimedia Foundation makes available logs of their web servers at https://dumps.wikimedia.org/. The data and format we're interested in is described in more detail on [this page](https://wikitech.wikimedia.org/wiki/Analytics/Archive/Data/Pagecounts-all-sites). In a nutshell, the files contain lines of data containing a small number of fields:

domain page_title count_views total_response_size
We will be looking at the data from August 3rd, 2016: https://dumps.wikimedia.org/other/pagecounts-raw/2016/2016-08/pagecounts-20160803-090000.gz

======


```
$ wikistats -h
 -b           only print 'total bytes' stats
 -d [domain]  if not specified, default to 'en'
              note: the special domain 'all' is also valid
 -f           only print 'most frequent' stats
 -h           print this help and exit
 -l           only print 'largest object' stats
 -r           only print 'requests per second' stats
 -u           only print 'unique objects' stats
```
