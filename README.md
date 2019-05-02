# Credits

Original Scraper by Danny Chrastil (@DisK0nn3cT): https://github.com/DisK0nn3cT/linkedin-gatherer

Modified by @vysecurity

Patched by @stormyordos

# Requirements
```
pip install beautifulsoup4
pip install thready
```

# Change Log
[02-05-2019]
* Patch: compatibility with the new code changes on Linkedin (loginCsrfParam and login page URI)
* Included a sample LinkedInt.cfg


[v0.1 BETA 12-07-2017]
Additions:
* UI Updates
* Constrain to company filters
* Addition of Hunter for e-mail prediction

# To-Do List

* Allow for horizontal scraping and mass automated company domain, and format prediction per company
* Add Natural Language Processing techniques on titles to discover groups of similar titles to be stuck into same "department". This should then be visualised in a graph.

# Usage

Put in LinkedIn credentials in LinkedInt.py
Put Hunter.io API key in LinkedInt.py
Run LinkedInt.py and follow instructions

# Example

```
██╗     ██╗███╗   ██╗██╗  ██╗███████╗██████╗ ██╗███╗   ██╗████████╗
██║     ██║████╗  ██║██║ ██╔╝██╔════╝██╔══██╗██║████╗  ██║╚══██╔══╝
██║     ██║██╔██╗ ██║█████╔╝ █████╗  ██║  ██║██║██╔██╗ ██║   ██║
██║     ██║██║╚██╗██║██╔═██╗ ██╔══╝  ██║  ██║██║██║╚██╗██║   ██║
███████╗██║██║ ╚████║██║  ██╗███████╗██████╔╝██║██║ ╚████║   ██║
╚══════╝╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝╚══════╝╚═════╝ ╚═╝╚═╝  ╚═══╝   ╚═╝

Providing you with Linkedin Intelligence
Author: Vincent Yiu (@vysec, @vysecurity)
Original version by @DisK0nn3cT
[*] Enter search Keywords (use quotes for more percise results)
"General Motors"

[*] Enter filename for output (exclude file extension)
generalmotors

[*] Filter by Company? (Y/N):
Y

[*] Specify a Company ID (Provide ID or leave blank to automate):


[*] Enter e-mail domain suffix (eg. contoso.com):
gm.com

[*] Select a prefix for e-mail generation (auto,full,firstlast,firstmlast,flast,first.last,fmlast):
auto

[*] Automaticly using Hunter IO to determine best Prefix
[!] {first}.{last}
[+] Found first.last prefix
```
