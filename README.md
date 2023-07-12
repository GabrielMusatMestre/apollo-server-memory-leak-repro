# Steps

Install the dependencies:
```bash
npm i
```

Run the server using a correctly configured APOLLO_KEY and APOLLO_GRAPH_REF:
```bash
APOLLO_KEY="<key>" APOLLO_GRAPH_REF="<ref>" node server.mjs
```

Make requests in a loop and see how the memory increases:
```bash
while true; do curl -X POST http://localhost:4000 -d '{"query": "query ExampleQuery { hello }"}' -H 'content-type: application/json'; done
```
