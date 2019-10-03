# Development

Some of the tools in the [DevOps](devops.md) page are obviously development tools, like Docker, but given their critical role in DevOps we decided to let them stay over there. We imagine this as a spot for things that reside on your laptop or on the web that assist in creating and developing digital products of some kind. Also, see [Non-Data Python](non-data-python.md) for Python language-specific resources.

## Text Editors

- [Visual Studio Code](https://code.visualstudio.com/) - unbelievably, an **OPEN-SOURCE MICROSOFT PRODUCT**. Not surprisingly, it's therefore a Microsoft product that not only doesn't suck but is really pretty awesome. This has become many people's new go-to text editor. Available for Windows (of course), Mac, and Linux.
- [VS Code Extension Marketplace](https://marketplace.visualstudio.com/vscode) - You name it, there's probably an extension for it. Want to Lint HTML? PHP? Python? Connect to an FTP server? All there.
- [Vim](https://www.vim.org/) - The OG text editor. Many hardcore developers will use nothing else. The learning curve is excrutiatingly steep (you use `H`, `J`, `K`, and `L` to move around, for instance), but it does inculcate an incredibly kind of efficiency. Check out the [Interactive VIM Tutorial](https://www.openvim.com/) to get a guided tour. Also, [this article](https://dn.ht/intermediate-vim/) is a good guide to 'Intermediate VIM.'
- [Sublime Text 3](https://www.sublimetext.com/3) - Formerly the best text editor in the world. Possibly supplanted by .
- [Package Control](https://packagecontrol.io/) - a HUGE ecosystem of plugins for Sublime Text. One of the principal reasons to use Sublime, but has largely been supplanted by the VS Code ecosystem.
- [Coder.com](https://coder.com/) - Visual Studio Code, but hosted on the web and in your browser. Very generous free plan.

## Database

- [DBeaver](https://dbeaver.io) - "Universal Database Tool" - "Free multi-platform database tool for developers, SQL programmers, database administrators and analysts. Supports all popular databases: MySQL, PostgreSQL, MariaDB, SQLite, Oracle, DB2, SQL Server, Sybase, MS Access, Teradata, Firebird, Derby, etc." GUI doesn't look terrible.
- [Flyway](https://flywaydb.org/) - "Version control for your database. Robust schema evolution across all your environments. With ease, pleasure (sic) and plain SQL." Lack of Oxford Comma aside, a cool tool for intelligently developing and deploying database schema changes.

## Code Analysis

- [Infer](https://fbinfer.com/) - I know we have some Java and some C and some C# developers in the State. Infer could be helpful. Here's how it works: "if you give Infer some Java or C/C++/Objective-C code it produces a list of potential bugs. Anyone can use Infer to intercept critical bugs before they have shipped to users, and help prevent crashes or poor performance." From Facebook.
- [Pyre](https://pyre-check.org/) - Also from Facebook, a type-checker for Python. Method says it's going to kick back an `int`, but it kicks back a `str` instead? Pyre will tell you this before you try to use it somewhere.

## API Design

- [OpenAPI](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md) - The homepage for /about the OpenAPI standard, which standardizes and helps automate the design of modern APIs.
- [OpenAPI Tools](https://openapi.tools/) - A compendium of tools to assist in the construction of modern APIs along the OpenAPI standard.
- [Stoplight Studio](https://stoplight.io/studio/) - A GUI for designign open API specs.

## Specialty

- [Expresso](http://www.ultrapico.com/) - We (maybe) all know that regular expressions are incredibly powerful and **fast** tools for finding things in text. They're also difficult to master. That's why Expresso is great, because it has a GUI to help you construct the right RegEx to filter/find exactly what you want. It's amazing that no other tool online or offline that I've found does this quite as well. It also has pre-built "formulas," like the RegEx for finding Zip Codes. `(?<Zip>\d{5})-(?<Sub>\d{4})`, turns out.
- [Regex101](https://regex101.com/) - A site that does a lot of what Expresso does. Has a handy quick reference guide in the bottom right. Put your regex in the top using the symbols in the quick reference guide, and paste in the data you want to search in to see what would come up using your RegEx expression. Pretty slick.
