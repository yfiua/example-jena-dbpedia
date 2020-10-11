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

## Note

When running the jar file, if you see
```
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
```
This only means the logger SLF4J is missing, and does not really matter.
