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

- [Scrapy](https://scrapy.org/) - An alternative to everything I just wrote above, this package is designed to 

## Code Formatting

- Less a tool, but more of the Bible for how to format/style Python code is [PEP8](https://www.python.org/dev/peps/pep-0008/?). *PEP* stands for *Python Enhancement Proposal*. This particular PEP was written by the creator of Python himself, [Guido van Rossum](https://gvanrossum.github.io/). In it, he makes the point that "code is read much more often than it is written." As such, code should be readable by humans.
- [Black](https://github.com/ambv/black) is an extremely-opinionated code formatter. To quote the project's site, "*Black* reformats entire files in place. It is not configurable. It doesn’t take previous formatting into account." But it's actually got a great aesthetic taste. Worth your time. Also has plugins to autoformat your code in a bunch of different editors.
- [iSort](https://pypi.org/project/isort/) - Will intelligently and elegantly sort your module imports at the top of your .py file. Compatible with Black.



## Reference

- [strftime.org](http://strftime.org/) - A handy little site for getting you exactly what you need. In this instance, a reminder of how to format the % sign and a bunch of letters to generate a date in the proper format. For example, `%Y-%m-%d`, in the right command, will generate `2018-07-24`.