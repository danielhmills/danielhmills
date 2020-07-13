Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
- 📫 How to reach me: [@danhmills.twitter](http://twitter.com/dan_hmills#this) (Twitter), [@danhmills.linkedin](https://www.linkedin.com/in/daniel-heward-mills-a0940465#this) (LinkedIn), [@danhmills.email](mailto:didehen@openlinksw.com) (Email)

- 💬 Ask me about ... [Knowledge Graph](https://twitter.com/hashtag/KnowledgeGraph), [Linked Data](https://twitter.com/hashtag/LinkedData), [ODBC](https://twitter.com/hashtag/ODBC), [JDBC](https://twitter.com/hashtag/JDBC), [Data Connectivity](https://twitter.com/hashtag/DataConnectivity), [WebID](https://twitter.com/hashtag/WebID)

## JSON-LD Start ##

{
  "@context": {
    "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
    "foaf": "http://xmlns.com/foaf/0.1/",
    "schema": "http://schema.org/",
    "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
    "dcterms": "http://purl.org/dc/terms/",
    "xsd": "http://www.w3.org/2001/XMLSchema#",
    "owl": "http://www.w3.org/2002/07/owl#",
    "cert": "http://www.w3.org/ns/auth/cert#"
  },
  "@graph": [
    {
      "@id": "",
      "@type": "foaf:PersonalProfileDocument",
      "foaf:maker": {
        "@id": "#i"
      },
      "foaf:primaryTopic": {
        "@id": "#i"
      }
    },
    {
      "@id": "#i",
      "@type": [
        "schema:Person",
        "foaf:Person"
      ],
      "schema:mainEntityOf": [
        {
          "@id": ""
        },
        {
          "@id": "https://www.linkedin.com/in/daniel-heward-mills-a0940465#"
        },
        {
          "@id": "https://www.twitter.com/dan_hmills#"
        }
      ],
      "schema:name": {
        "@type": "rdf:langString",
        "@value": "Daniel Heward-Mills"
      },
      "owl:sameAs": [
               {
          "@id": "https://www.linkedin.com/in/daniel-heward-mills-a0940465#"
        },
        {
          "@id": "https://www.twitter.com/dan_hmills#"
        }
      ]
    },
    {
      "@id": "https://raw.githubusercontent.com/danielhmills/danielhmills/master/README.md#this",
      "@type": [
        "foaf:Document",
        "schema:WebPage"
      ],
      "dcterms:created": {
        "@type": "xsd:dateTime",
        "@value": "2020-07-13"
      },
      "dcterms:creator": {
        "@id": "#i"
      },
      "schema:mainEntity": {
        "@id": "#i"
      },
      "rdfs:name": {
        "@type": "rdf:langString",
        "@value": "Daniel Heward-Mills's Profile Document"
      },
      "foaf:primaryTopic": {
        "@id": "#i"
      }
    }
  ]
}

## JSON-LD End ##

```

Here is the same Profile Information using [RDF-Turtle](https://medium.com/openlink-software-blog/simple-linked-data-deployment-tutorial-a532e568c82f) Notation. 

```
## Turtle Start ##

@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix schema: <http://schema.org/> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix cert: <http://www.w3.org/ns/auth/cert#> . 
@prefix : <#> . 

# Profile Document Metadata
<> rdf:type foaf:Document, foaf:PersonalProfileDocument, schema:WebPage, schema:CreativeWork .
<> foaf:maker :i .
<> foaf:primaryTopic :i .
<> schema:mainEntity :i .
<> schema:dateCreated "2020-07-13"^^xsd:dateTime .
<> schema:creator :i .
<> schema:name "Daniel Heward-Mills's Profile Document" .

# Personal Information 
:i schema:mainEntityOf <> .
:i schema:mainEntityOf <https://www.linkedin.com/in/daniel-heward-mills-a0940465#> .
:i schema:mainEntityOf <https://www.twitter.com/dan_hmills#> .
:i rdf:type schema:Person, foaf:Person .
:i schema:name "Daniel Hewawrd-Mills" .
:i owl:sameAs <https://www.linkedin.com/in/daniel-heward-mills-a0940465#this> .
:i owl:sameAs <https://www.twitter.com/dan_hmills#this> .

## Turtle End ##
