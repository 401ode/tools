# Non Data-Related Python Stuff

It's no secret that one of the writers (@bmcguirk) of this repository really likes [Python](http://www.python.org). He wants you to, as well, because it has improved his life since he started learning it. We also need more people in State government fluent in this kind of thing.

To get started, we recommend the [Anaconda distribution](https://www.anaconda.com/distribution/) of Python. It's pre-packed with 1,400+  great modules that are pre-compiled and pre-configured for your operating system. These modules are geared towards doing science in Python, but we think it's worth it to get the full kit and caboodle. So what if you never use [Astropy](http://www.astropy.org/) in your day-to-day work for the State. There are still hundreds of useful modules in there.

## Training

- [The Freaking NSA's Intro to Python Handbook!](https://nsa.sfo2.digitaloceanspaces.com/comp3321.pdf) - The result of a [FOIA Request](https://twitter.com/chris_swenson/status/1225836060938125313). Just in case that link ever goes away, it's been uploaded to the [Internet Archive](https://archive.org/details/comp3321/page/n4/mode/2up).
- [Interactive Coding Challenges](https://github.com/donnemartin/interactive-coding-challenges) - Really pretty comprehensive. Also difficult.

## Web / HTML

- [`BeautifulSoup`](https://www.crummy.com/software/BeautifulSoup/) - HTML Parsing made super easy. But it needs to be fed HTML. You could use Python's built-in `urllib` or `httplib`, but what you really want to use is...
- [`requests`](http://docs.python-requests.org/en/master/), which describes itself as "HTTP for Humans." From like 8 lines of code to go grab the content of a website, you just `import requests` and then `requests.get('https://github.com/401ode/tools`. Now the whole content of that request is an a Pythonic object, which you can then feed to BeautifulSoup to parse and do whatever you want with. Like if you want to get all the links out of a given page, you just do:

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

- [`Scrapy`](https://scrapy.org/) - An alternative to everything I just wrote above, this package is designed to intelligently scrape whatever site you point it at. Seems super-promising.

## Code Formatting

- Less a tool, but more of the Bible for how to format/style Python code is [PEP8](https://www.python.org/dev/peps/pep-0008/?). *PEP* stands for *Python Enhancement Proposal*. This particular PEP was written by the creator of Python himself, [Guido van Rossum](https://gvanrossum.github.io/). In it, he makes the point that "code is read much more often than it is written." As such, code should be readable by humans.
- [`yapf`](https://github.com/google/yapf) - Google's opinionated code-formatter. To wit: 'Most of the current formatters for Python --- e.g., `autopep8`, and `pep8ify` --- are made to remove lint errors from code. This has some obvious limitations. For instance, code that conforms to the PEP 8 guidelines may not be reformatted. But it doesn't mean that the code looks good... YAPF takes a different approach. It's based off of `clang-format`, developed by Daniel Jasper. In essence, the algorithm takes the code and reformats it to the best formatting that conforms to the style guide, even if the original code didn't violate the style guide. The idea is also similar to the `gofmt` tool for the Go programming language: end all holy wars about formatting...'
- [`black`](https://github.com/ambv/black) is an extremely-opinionated code formatter. To quote the project's site, "*Black* reformats entire files in place. It is not configurable. It doesn’t take previous formatting into account." But it's actually got a great aesthetic taste. Worth your time. Also has plugins to autoformat your code in a bunch of different editors.
- [`iSort`](https://pypi.org/project/isort/) - Will intelligently and elegantly sort your module imports at the top of your .py file. Compatible with Black.

## Image Manipulation

### Image Manipulation Modules

- [`pillow`](https://pillow.readthedocs.io/en/5.2.x/) - A fork of an old-school, but incredibly powerful, project called Python Imaging Library or PIL, this is much easier to use and just as powerful.
- [OpenCV for Python](https://docs.opencv.org/3.3.0/d0/de3/tutorial_py_intro.html) - An old-school, but incrediby powerful, "Computer Vision" system. It takes a bit of work to get it installed on Windows ([see this guide])(https://www.learnopencv.com/install-opencv3-on-windows/), but then it offers some very powerful ways to get your computer to "see."

### Image Manipulation Guides

- [Creating GIFS with OpenCV](https://www.pyimagesearch.com/2018/11/05/creating-gifs-with-opencv/) - a tongue-in-cheek guide/tutorial, but teaches some very cool techniques for image manipulation and creation.

## Cool Built-In Modules

- [`re`](https://docs.python.org/3/library/re.html) - Excellent and flexible use of regular expressions.
- [`collections`](https://docs.python.org/3/library/collections.html) - A bunch of different collectio objects. New favorite one is [Counter](https://docs.python.org/3/library/collections.html#collections.Counter), where you can feed in elements and it'll keep track of how frequently they are used.
- [`random`](https://docs.python.org/3/library/random.html) - "This module implements pseudo-random number generators for various distributions." They note, however, that "the pseudo-random generators of this module should not be used for security purposes. For security or cryptographic uses, see the [`secrets`](https://docs.python.org/3/library/secrets.html#module-secrets) module."

## Distribution

- [Making a PEX from a Python Script](https://peterdemin.github.io/script-to-pex.html) - Lovely guide for getting around the "that script is great but I don't have python installed on my computer" issue. Copiling a PEX will take all the dependencies, the Python engine, etc. and pack it into a one-shot executable file.

## Reference

- [strftime.org](http://strftime.org/) - A handy little site for getting you exactly what you need. In this instance, a reminder of how to format the % sign and a bunch of letters to generate a date in the proper format. For example, `%Y-%m-%d`, in the right command, will generate `2018-07-24`.
- [Comprehensive Python Cheat Sheet](https://gto76.github.io/python-cheatsheet/) - Holy moly, comprehsnive is right. [Here's](https://github.com/gto76/python-cheatsheet) the link to the Github Repo.

## Testing

- [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) - "Hypothesis is a Python library for creating unit tests which are simpler to write and more powerful when run, finding edge cases in your code you wouldn’t have thought to look for. It is stable, powerful and easy to add to any existing test suite... It works by generating arbitrary data matching your specification and checking that your guarantee still holds in that case. If it finds an example where it doesn’t, it takes that example and cuts it down to size, simplifying it until it finds a much smaller example that still causes the problem. It then saves that example for later, so that once it has found a problem with your code it will not forget it in the future." Very cool.