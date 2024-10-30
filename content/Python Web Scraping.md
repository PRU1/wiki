[[Getting info from user screen in Python]]

[A Practical Introduction to Web Scraping in Python – Real Python](https://realpython.com/python-web-scraping-practical-introduction/)

- collecting and parsing raw data from the web
- websites may limit web scraping with automated tools
	- i.e. repeating requests can eat up bandwidth

```
>>> from urllib.request import urlopen
```

open url
```
url = "https://website_name"
page = urlopen(url)
```

`urlopen()` returns an HTTPResponse object --> the response a server responds back to a client in [[HTTP Protocol]]

- you have to read and decode website (info provided in attached web link)