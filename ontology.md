## Ontology Documentation


This is the main ontology document. All other representations are generated automatically from this document.

- [Turtle](ontology.ttl)

### Namespaces
The following namespaces are used in this ontology:

```
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix gndo: <http://d-nb.info/standards/elementset/gnd#> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix geo: <http://www.opengis.net/ont/geosparql#> .
@prefix tan: <http://tanhuma.com/ontology#> .
```

### Concept
Class: tan:Artifact

* Title
* Type
    * Manuscripts
    * Printed Editions
    * Genizah Fragments
    * Binding Fragments

* Definitiion
* tagging format

### lections
* Parasha
* Seder
* special Reading
* Name = label
* opening verse

### biblical reference
* books
* chapter
* verse
* word
* sequence

  ### canonical editions
  * label, e.g. "Pesiqta rabbati 34:5"
  * 

### rabbinic reference
* canonical edition
* citation
* parallel

#### rabbinical citation
* label@en
* henLabel@he


### Entities
* type
* label
* prefLabel
* hebrew

Class: tan:codicologicalUnits

Class: structuralUnits
label@en
label@he
uuid

Unit:
* [Proem](https://github.com/Tahuma/ontology/wiki/Proem)
* Body
* Peroration

#### Unit sub type
Halakhic 
ZS"H
Circular
Above
Exegesis
Narrative Midrash



### Concept

Class: skos:Concept


#### skos:altLabel
```
skos:altLabel
    a rdf:Property ;
    rdfs:label "alternative label"@en ;
    rdfs:comment "Alternative writing format or language of the preferred label of a person or concept"@en ;
    rdfs:range rdfs:Literal .
```
#### skos:prefLabel
```
skos:prefLabel
    a rdf:Property ;
    rdfs:label "preferred label"@en ;
    rdfs:comment "The label that is preferred to be used for a person or concept"@en ;
    rdfs:range rdfs:Literal .
```
#### skos:related
```
skos:related
    a rdf:Property ;
    rdfs:label "has related"@en ;
    rdfs:comment "used to assert an associative link between two skos concepts"@en ;
    rdfs:range skos:Concept .
```
#### skos:scopeNote
```
skos:scopeNote
    a rdf:Property ;
    rdfs:label "scope note"@en ;
    rdfs:comment "Notes are used to provide information relating to skos concepts"@en ;
    rdfs:range rdfs:Literal .
```
#### skos:broader
```
skos:broader
    a rdf:Property ;
    rdfs:label "has broader"@en ;
    rdfs:comment "used to indicates that one skos concept is in some way more general (broader) than the other"@en  ;
    rdfs:range skos:Concept .
```
#### skos:narrower
```
skos:narrower
    a rdf:Property ;
    rdfs:label "has narrower"@en ;
    rdfs:comment "used to indicates that one skos concept is in some way less general (narrower) than the other"@en ;
    rdfs:range skos:Concept .
```


#### dcterms:identifier
```
dcterms:identifier
    a rdf:Property ;
    rdfs:label "identifier"@en ;
    rdfs:comment "An unambiguous reference to the resource within a given context"@en ;
    rdfs:range rdfs:Literal .
```
#### dcterms:subject
```
dcterms:subject
    a rdf:Property ;
    rdfs:label "subject"@en ;
    rdfs:comment "The topic of the resource, category or subject heading that further describes this resource. (broader category used to describe ) "@en ;
    rdfs:range owl:Thing .
```

#### geo:asWKT
```
geo:asWKT
    a rdf:Property ;
    rdfs:label "asWKT"@en ;
    rdfs:comment "The WKT serialization of a geometry"@en ;
    rdfs:range geo:wktLiteral .
```


### Document

Class: foaf:Document

#### foaf:primaryTopic
```
foaf:primaryTopic
    a rdf:Property ;
    rdfs:label "primary topic"@en ;
    rdfs:comment "The primary topic of some page or document"@en ;
    rdfs:range owl:Thing .
```
#### rdfs:label
```
rdfs:label
    a rdf:Property ;
    rdfs:label "label"@en ;
    rdfs:comment "used to provide a human-readable version of a resource's name"@en ;
    rdfs:range rdfs:Literal .
```
#### dcterms:created
```
dcterms:created
    a rdf:Property ;
    rdfs:label "created"@en ;
    rdfs:comment "Date of creation of the resource"@en ;
    rdfs:range rdfs:Literal .
```

### Metadata

The Tanhuma Project ontology is maintained on Github via the following document:

[https://github.com/wisslab/judaicalink-ontology/blob/master/judaicalink-ontology.md](
https://github.com/wisslab/judaicalink-ontology/blob/master/judaicalink-ontology.md)

You can create comments on the file and/or raise an [issue](https://github.com/wisslab/judaicalink-ontology/issues).

