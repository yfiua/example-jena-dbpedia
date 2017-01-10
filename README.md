# example-jena-dbpedia

It runs the following SPARQL query:
```
SELECT ?prop ?place WHERE { <http://dbpedia.org/resource/%C3%84lvdalen> ?prop ?place .}
```

Expected result:

```
-----------------------------------------------------------------------------------
| prop                                   | place                                  |
===================================================================================
| <http://www.w3.org/2002/07/owl#sameAs> | <http://dbpedia.org/resource/Älvdalen> |
-----------------------------------------------------------------------------------
```
