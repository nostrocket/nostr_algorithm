## nostr algorithm design

This repo is part of a nostr recommendation engin project. It crawl data from relays and store useful information in graph database (neo4j). In the db every npub and event is a node. if a npub like/repost/zap an event, there will be an edge created between this npub and event. Different user behavior will add different weight to the edge. The algorithm of calculating node similarity is documented in [here](https://neo4j.com/docs/graph-data-science/current/algorithms/node-similarity/)

## To do

- [ ] delete bot part to simplify the project(create a bot is not the main foucus, might use relat feed in the future)
- [ ] set up test env on vps to store longer structured data
- [ ] add new handler to return similarity for given npub 
- [ ] add relay feed
- [ ] add more user behavior (comment, share, bookmark)
- [ ] parse historical event (1.25 TB one)
- [ ] add wot filter
- [ ] explore different data structure to store event for similarity calculation
- [ ] add text based analysis using llm 