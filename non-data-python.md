# Non Data-Related Python Stuff

It's no secret that one of the writers (@bmcguirk) of this repository likes [Python](http://www.python.org). He wants you to, as well, because it has actively improved his life since he started learning it. We also need more people in State government fluent in this kind of thing. 

## Web / HTML
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) - HTML Parsing made super easy. But it needs to be fed HTML. You could use Python's built-in `urllib` or `httplib`, but what you really want to use is...
- [Requests](http://docs.python-requests.org/en/master/), which describes itself as "HTTP for Humans." From like 8 lines of code to go grab the content of a website, you just `import requests` and then `requests.get('https://github.com/401ode/tools`. Now the whole content of that request is an a Pythonic object, which you can then feed to BeautifulSoup to parse and do whatever you want with. Like if you want to get all the links out of a given page, you just do: 

```python
import requests
from bs4 import BeautifulSoup as bs

odetools = requests.get('https://github.com/401ode/tools')
odetoolsoup = bs(odetools.content, 'html.parser')

for link in odetoolsoup.find_all('a'):
    print(link.get('href'))
# http://example.com/brian
# http://example.com/ryan
# http://example.com/shawn
```

## 