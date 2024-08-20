
## Fire up jinaga
(Depends on docker destkop with docker-compose)

`$> docker-compose up jinaga_replicator`

## Submit fact graph to write endpoint

`$> curl -vv -X POST --data "@/Users/dkichler/sandbox/immutable-architecture/blog-facts.fml" -H "Content-Type: text/plain" http://127.0.0.1:8080/jinaga/write`

## Submit blog post spec to read endpoint

`$> curl -vv -X POST --data "@/Users/dkichler/sandbox/immutable-architecture/blog-post-spec.fml" -H "Content-Type: text/plain" http://127.0.0.1:8080/jinaga/write`
