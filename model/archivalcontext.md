<!---

BIBFRAME EAC-CPF is a starting point for archival vocabularies using the 
http://bibfra.me model and profiles. It builds off of the BIBFRAME Lite vocabulary 
and Encoded Archival Context—Corporate Bodies, Persons, and Families (EAC-CPF).
It is framework conformant to BIBFRAME and where possible, link-compatible 
with the Library of Congress's BIBFRAME vocabulary, http://bibframe.org/

BIBFRAME context is expressed using the Versa data model, which also
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

template 

# lowerCase/UpperCase

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark: 

--> 

<!---

For definitions see: http://eac.staatsbibliothek-berlin.de/fileadmin/user_upload/schema/cpfTagLibrary.html

--> 

<!---

Terms below are elements mapped from EAC-CPF

-->

## abbreviation

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark: 


## abstract

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

## addressLine 

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark: 

## addressLine 

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## agencyCode 

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## agencyName 

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

## agentType

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## alternativeForm

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## alternativeSet

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## authorizedForm

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## biogHist

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## chronItem

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## chronList

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

## componentEntry

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

## conventionDeclaration   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## cpfDescription

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## cpfRelation

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

## dateRange

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## dateSet

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## description

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## descriptiveNote

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## eaccpf

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## entityId

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## entityType

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

## eventDateTime

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## eventDescription

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## eventType   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## existDates

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## fromDate

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

## functionRelation

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## functions

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## generalContext

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## identity   

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

## language

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## languageDeclaration

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## languagesUsed

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## languageUsed

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## legalStatus

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## legalStatuses

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## level

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

## localControl

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## localDescription

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## localDescriptions

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## localTypeDeclaration   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenanceAgency

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenanceEvent

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenanceHistory

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## maintenanceStatus

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## mandate   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## mandates

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## multipleIdentities

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## nameEntry

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## nameEntryParallel   

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

## occupations

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## otherAgencyCode

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## otherRecordId

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## outline  

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

## place   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## placeEntry

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## placeRole

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## places

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## preferredForm

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## publicationStatus

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## recordId

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## relationEntry

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

## resourceRelation

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

## setComponent

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

## sourceEntry

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

## span   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## structureOrGenealogy

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

## toDate   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## useDates  

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:


<!---

Terms below are attributes mapped from EAC-CPF

-->

## accuracy

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## altitude

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## countryCode

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## cpfRelationType

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## functionRelationType 

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## identityType

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## languageCode

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## lastDateTimeVerified

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## latitude

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## localType

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## longitude   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## notAfter

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## notBefore

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## resourceRelationType

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## scriptCode

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## standardDate

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## standardDateTime   

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## style

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## transliteration

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

## vocabularySource    

* label: 
* refines: <http://bibfra.me/vocab/lite/xxxx>
* synonyms: 
* description: 
* value: Literal/resource
* properties:  
* scope: <http://bibfra.me/vocab/archive>
* remark:

<!---

Unmapped EAC-CPF Elements: 
* objectXMLWrap
* objectBinWrap

Unmapped EAC-CPF Attributes: 
* xlink:actuate
* xlink:arcrole
* xlink:href
* xlink:role
* xlink:show
* xlink:title
* xlink:type
* xml:base
* xml:id
* xml:lang

-->
