Bulk Bing Image Downloader
==========================
*Bulk Bing Image Downloader (BBID)* is downloader which:
- Downloads full-size images from bing image search results
- Is asynchronous -> downloads images super fast
- Is crossplatform
- Bypasses Bing API
- Has option to disable adult content filtering
- Is written in python 3.
- Uses SSL connection

## Installation

```sh
pip install git+https://github.com/fede-h/bulk-bing-image-downloader
```

### Usage
```
usage: bbid.py [-h] [-f] [-o OUTPUT] [-a] [-g] [--filters FILTERS] [--limit LIMIT] [-t THREADS]
               search_string [search_string ...]

Bing image bulk downloader

positional arguments:
  search_string         Keyword to search

optional arguments:
  -h, --help            show this help message and exit
  -f, --search-file     search-string is a path to a file containing search strings line by line
  -o OUTPUT, --output OUTPUT
                        Output directory
  -a, --adult-filter-off
                        Disable adult filter
  -g, --animated-gif    Disable adult filter
  --filters FILTERS     Any query based filters you want to append when searching for images, e.g. +filterui:license-L1  
  --limit LIMIT         Make sure not to search for more than specified amount of images.
  -t THREADS, --threads THREADS
                        Number of threads
```
Or if you would like, you can watch [YouTube tutorial](https://youtu.be/nJ4CixTsYQI)

### Example

`bbid hello world`

For advanced filters reference guide, check `filters_guide.md`
