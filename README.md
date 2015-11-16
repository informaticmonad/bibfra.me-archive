bibfra.me Vocabulary for Archival Description
========

The vocabulary in this respository reflects [Zepheira's](http://zepheira.com) approach
to [modular, layered vocabulary management] (http://bibfra.me).  The vocabulary is being shaped by a range
of related professional services engagements along with help from participants
in Zepheira's [Practical Practitioner, Linked Data training series](http://zepheira.com/solutions/library/training/) and volunteers from other communities of librarians and archvisits. All vocabulary development is based on use-cases and test data.

The vocabulary evolves and works alongside our data diagnostics, transformation and enhancement services,
along with the [Libhub inititative](http://libhub.org) to make libraries and archives visible on the Web. The [core implementation of these services is available as open source software](https://github.com/zepheira/pybibframe).

Please let us be clear that these vocabularies are not intended to replace or compete with other Linked Data
namespaces, for libraries, archives, or any other purpose. These vocabularies take advantage of BIBFRAME profiles,
and are designed to be enhanced by layering on further profiles, perhaps to represent the needs of a particular
institution, consortium or area of usage specialization. We hope that by sharing this approach, others may consider
similar practices for effective vocabulary management and distributed governance, through the the flexibility of
BIBFRAME.

See also: [Library of Congress's BIBFRAME site](http://bibframe.org/)

Representation
========

The main files of interest are in the directory `model`. Each one contains the vocabulary for one of the layers/profiles which can be used independently. They are in a format called Versa Literate, which is based on Markdown. Versa Literate is designed for easy reading and edit by even non-technical people. Here is a brief guide.

```
# @docheader

* @base: http://bibfra.me/vocab/
* @property-base: http://bibfra.me/purl/versa/support
* title: Lite version of BIBFRAME vocabulary
```

A special section serving as a document header. `@base` is the default base IRI, used e.g. for resource headers (see below). It would also be used for properties except that in this case it is overridden by `@property-base`, which specifies a base IRI for properties.

```
# Resource

* synonyms: http://bibframe.org/vocab/Resource http://schema.org/Thing
* label: Resource
* description: Conceptual Resource
* properties: label description image link
```

A section defining a resource type (analogous to an RDF class), as indicated by convention in this case by a top-level header marker (`#`). The List (multiple lines starting with (`*` then space) defines properties of the resource, or really metaproperties in this case.

```
## property

* description: a relationship between two resources or a resource and literal data
* label: property
```

A section defining a property (analogous to an RDF property), as indicated by convention in this case by a second-level header marker (`##`). Again the List defines metaproperties of the property.


Contributing
========

If you are interested in contributing or collaborating, please contact Gloria Gonzalez - gloria (at) zepheira (dot) com

Contributors:
* Gloria Gonzalez, Library Strategist at Zepheira 
* Alexis Antracoli, Assistant University Archivst and Archivst for Technical Services at Princeton University
