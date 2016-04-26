# mongo-crawler

## Overview

*mongo-crawler* is a coordinated, agent-based, distributed web crawler. 

*mongo-crawler* is a protocol specifying how the agents communicate and collaborate.
It is language independent, currently python2 implementation is offered.

The minimal set of agents that can perform web crawling task automatically, should consists of at least four types of agents: jobpcaker, collector, downloader, and parser.

*mongo-crawler* choose MongoDB as data storage, message queue and message bulletin board. 

*mongo-crawler* is designed in the flavor that all modules are loosely-coupled. This is the rationale of an agent-based architecture.

*mongo-crawler* is simple and should be simple, that it should be easy to read, easy to understand, easy to maintain and easy to extend.

At the same time, users and developers of *mongo-crawler* should keep in mind the responsibility to minimize the environmental impact caused by your traffic and connections. Technically, one should put engineering effort to minimize the number of connection, total bandwidth and total up/down as small as possible. Socially, one should always respect the rules and preferencce of every individual or organization that your crawler will visist, honor robots.txt and set appropriate politeness_interval.

## Package Dependency

This section describes package dependency of *python2-mongo-crawler*, since it is the only implementation of *mongo-crawler* at this time point.

* Python 2.6 or newer
* MongoDB 3.2 or newer (possibly compatible to 3.0, not tested) <a href="https://www.mongodb.org/downloads#production">download</a>,  <a href="https://docs.mongodb.org/manual/">doc</a>
* python2-pymongo
* python2-requests <a href="http://docs.python-requests.org/en/master/">http://docs.python-requests.org/en/master/</a>
* python2-lxml <a href="http://lxml.de/">http://lxml.de/</a>
* python2-beautifulsoup4 <a href="https://www.crummy.com/software/BeautifulSoup/bs4/doc/">https://www.crummy.com/software/BeautifulSoup/bs4/doc/</a>

If you replace the existing component with your own implementation, python2-requests (for downloader), python2-lxml (for parser), python2-beautifulsoup4 (for parser) may not be required.

