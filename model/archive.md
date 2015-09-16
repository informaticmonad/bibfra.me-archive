<!---

BIBFRAME Archive is a starting point for archival vocabularies using the 
http://bibfra.me model and profiles. It builds off of the BIBFRAME Lite vocabulary. 
It is framework conformant to BIBFRAME and . and where possible, link-compatible with the 
US Library of Congress's BIBFRAME vocabulary, http://bibframe.org/

BIBFRAME Archive is expressed using the Versa data model, which also
allows for full expression in RDF form.  This particular file is in
the Versa Literate syntax, based on the Markdown format
<https://daringfireball.net/projects/markdown/basics>.

The convention for expressing data models in Versa Literate has each
vocabulary item starting with a new header, A level 1 header for
resource classes and level 2 for properties.  Each has its ID as an
IRI reference (usually relative). Each is then described within its
section's unordered list, given a "label" (display label),
"description" (also for explanatory display), possibly "synonyms" (one
or more loose expression that the resource can be considered a synonym
for another). Resource classes may also have "properties"
(space-separated list of property IDs defined on the
resource). Properties may also have "value" (textual description of
the expected value of the property, perhaps as a relationship to
another resource, or as a data value).

You'll notice that BIBFRAME Archive terms use a humpCase/HumpCase convention,
which derives from BIBFRAME legacy.

-->

# @docheader

<!---

@base is the default base IRI, used e.g. for resource headers. It
would also be used for properties except that it is overridden by
@property-base

The meta-properties in this file are actually defined by the Versa
data model to support interpretation by Versa modeling tools

@resource-base is another possible override, for resource headers, but
not used here

-->

* @iri:
    * @base: http://bibfra.me/vocab/archive/
    * @property: http://bibfra.me/purl/versa/support
* title: BIBFRAME Archive vocabulary
* @interpretations:
    * scope: @resource

<!---
Extend BIBFRAME Lite Classess
--->

# <http://bibfra.me/vocab/lite/Work>
* properties:  

# <http://bibfra.me/vocab/lite/Instance>
* properties: 

# <http://bibfra.me/vocab/lite/Authority>

# <http://bibfra.me/vocab/lite/Person>
* properties: 

# <http://bibfra.me/vocab/lite/Organization>
* properties: 

# <http://bibfra.me/vocab/lite/Meeting>
* properties: 

# <http://bibfra.me/vocab/lite/Topic>
* properties: 

# <http://bibfra.me/vocab/lite/Form>
* properties: 

<!---

Class Refinements 
-->


# findingAid

* label: finding aid
* refines: 
* synonyms: 
* description: A work with finding aid characteristics that describes archival collections to give the repository physical and intellectual control over the materials, and assist users in gaining access to and understanding the materials
* value: Literal
* properties: eadId 
* scope: <http://bibfra.me/vocab/archive>
* remark: 

<!---

Properties - [Terms below are mapped from Structural and Other Limited EAD Elements]

-->

## eadId

* label: EAD Identifier
* refines: <http://bibfra.me/vocab/lite/controlCode>
* synonyms: 
* description: Designates a unique code for a particular EAD finding aid document
* value: Literal
* scope: <http://bibfra.me/vocab/archive>
* remark: Equivalent to EAD ID <eadid>

<!---

EAD elements below are not mapped to the terms above: 

<ead> – EAD wrapper
<eadheader> – EAD Header
<filedesc> –  File Description 

-->

<!---

Terms below mapped from EAD3 elements

-->

## abbr



## abstract

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## accessrestrict

* label: Conditions Governing Access
* refines: <http://bibfra.me/vocab/lite/note>
* synonyms: http://bibframe.org/vocab/accessCondition.html
* description: Desginates whether or not there are any restrictions on the material, and states the nature of existing restrictions.
* value: Literal/resource
* properties:  end date
* scope: <http://bibfra.me/vocab/archive>
* remark:

## accruals

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## acqinfo

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## address

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## addressline

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## agencycode

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## agencyname

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## agent

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## agenttype

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## altformavail

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## appraisal

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## archdesc

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## archref

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## arrangement

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## author

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## bibliography

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## bibref

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## bioghist

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## blockquote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c01

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c02

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c03

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c04

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c05

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c06

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c07

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c08

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c09

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c10

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c11

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## c12

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## chronitem

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## chronitemset

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## chronlist

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## citation

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## colspec

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## container

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## control

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## controlaccess

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## controlnote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## conventiondeclaration

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## corpname

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## custodhist

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## dao

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## daoset

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## date

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## daterange

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## dateset

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## datesingle

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## defitem

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## descriptivenote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## did

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## didnote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## dimensions

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## dsc

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## ead

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## edition

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## editionstmt

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## emph

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## entry

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## event

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## eventdatetime

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## eventdescription

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## eventtype

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## expan

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## famname

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## filedesc

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## fileplan

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## footnote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## foreign

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## fromdate

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## function

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## genreform

## geogname

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## geographiccoordinates

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## head

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## head01

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## head02

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## head03

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## index

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## indexentry

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## item

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## label

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## langmaterial

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## language

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## languagedeclaration

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## languageset

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## lb

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## legalstatus

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## list

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## listhead

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## localcontrol

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## localtypedeclaration

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenanceagency

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenanceevent

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenancehistory

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenancestatus

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## materialspec

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## name

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## namegrp

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## notestmt

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## num

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## occupation

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## odd

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## originalsloc

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## origination

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## otheragencycode

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## otherfindaid

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## otherrecordid

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## p

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## part

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## persname

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## physdesc

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## physdescset

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## physdescstructured

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## physfacet

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## physloc

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## phystech

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## prefercite

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## processinfo

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## ptr

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## ptrgrp

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## publicationstatus

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## publicationstmt

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## publisher

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## quantity

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## quote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## recordid

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## ref

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## relatedmaterial

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## relation

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## relationentry

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## relations

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## repository

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## representation

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## row

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## scopecontent

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## script

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## separatedmaterial

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## seriesstmt

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## source

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## sourceentry

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## sources

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## sponsor

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## subject

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## subtitle

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## table

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## tbody

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## term

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## tgroup

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## thead

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## title

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## titleproper

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## titlestmt

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## todate

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## unitdate

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## unitdatestructured

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## unitid

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## unittitle

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## unittype

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## userestrict

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:
