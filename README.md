# example-jena-dbpedia

This is the simplest example to SPARQL-query DBpedia using Apache Jena. It runs the following SPARQL query:
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

## Build with Maven & Run

```
mvn package
java -jar target/examlple-jena-dbpedia-0.0.1-SNAPSHOT.jar 
```
