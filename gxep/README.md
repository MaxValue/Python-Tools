# GXEP
_a command line tool to search XML files for a given XPath expression_

## Status
Currently work in progress, the goal is to mimic grep as close as possible.

It can only parse HTML files for now.

## Small To-Do's:
* change usage message
* change epilog message
* use choices for query type (HTML or XML) flag

## Roadmap
1. Read XPath Queries from file
2. Read from STDIN
3 Support XML and provide a switch to handle XML/HTML respectively
4. Find out if the line number can be displayed, or at least a direct XPath to address the location of the match
5 Implement Python interface so this can be used as a module
6. Deploy to Pypi?
7. A GUI?
