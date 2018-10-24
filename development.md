# Development

Some of the tools in the [DevOps](devops.md) page are obviously development tools, like Docker, but given their critical role in DevOps we decided to let them stay over there. We imagine this as a spot for things that reside on your laptop or on the web that assist in creating and developing digital products of some kind. Also, see [Non-Data Python](non-data-python.md) for Python language-specific resources.

## Text Editors

- [Sublime Text 3](https://www.sublimetext.com/3) - For ODE's money, the best text editor in the world.
- [Package Control](https://packagecontrol.io/) - a HUGE ecosystem of plugins for Sublime Text. One of the principal reasons to use Sublime.
- [Visual Studio Code](https://code.visualstudio.com/) - unbelievably, an **OPEN-SOURCE MICROSOFT PRODUCT**. Not surprisingly, it's therefore a Microsoft product that doesn't actually suck. Also a huge ecosystem of plugins for everything imaginable.

## Database

- [DBeaver](https://dbeaver.io) - "Universal Database Tool" - "Free multi-platform database tool for developers, SQL programmers, database administrators and analysts. Supports all popular databases: MySQL, PostgreSQL, MariaDB, SQLite, Oracle, DB2, SQL Server, Sybase, MS Access, Teradata, Firebird, Derby, etc." GUI doesn't look terrible.
- [Flyway](https://flywaydb.org/) - "Version control for your database. Robust schema evolution across all your environments. With ease, pleasure (sic) and plain SQL." Lack of Oxford Comma aside, a cool tool for intelligently developing and deploying database schema changes.

## Code Analysis

- [Infer](https://fbinfer.com/) - I know we have some Java and some C and some C# developers in the State. Infer could be helpful. Here's how it works: "if you give Infer some Java or C/C++/Objective-C code it produces a list of potential bugs. Anyone can use Infer to intercept critical bugs before they have shipped to users, and help prevent crashes or poor performance." From Facebook.
- [Pyre](https://pyre-check.org/) - Also from Facebook, a type-checker for Python. Method says it's going to kick back an `int`, but it kicks back a `str` instead? Pyre will tell you this before you try to use it somewhere.

## Specialty

- [Expresso](http://www.ultrapico.com/) - We (maybe) all know that regular expressions are incredibly powerful and **fast** tools for finding things in text. They're also difficult to master. That's why Expresso is great, because it has a GUI to help you construct the right RegEx to filter/find exactly what you want. It's amazing that no other tool online or offline that I've found does this quite as well. It also has pre-built "formulas," like the RegEx for finding Zip Codes. `(?<Zip>\d{5})-(?<Sub>\d{4})`, turns out.
