# mongo-crawler

# Overview

*mongo-crawler* is a coordinated, agent-based, distributed web crawler. 

*mongo-crawler* is a protocol specifying how the agents communicate and collaborate.
It is language independent, currently offers python implementation.

The minimal set of agents that can perform web crawling task automatically, should consists of at least four types of agents: jobpcaker, collector, downloader, and parser.

*mongo-crawler* choose MongoDB as data storage, message queue and message bulletin board. 

*mongo-crawler* is designed in the flavor that all modules are loosely-coupled. This is the rationale of an agent-based architecture.

*mongo-crawler* is simple and should be simple, in the sense that it should be easy to read, easy to understand, easy to maintain and easy to extend.

At the same time, users and developers of *mongo-crawler* should keep in mind the responsibility to minize the environmental impact caused by your traffic and connections. Technically, one should put engineering effort to minize the number of connection, total bandwidth and total up/down as small as possible. Socially, one should always respect the rules and preferencce of every individual or organization that your crawler will visist, honor robots.txt and set appropriate politeness_interval.


