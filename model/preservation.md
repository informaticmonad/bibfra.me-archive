<!---

BIBFRAME Preservation is a starting point for preservation vocabularies using the 
http://bibfra.me model and profiles. It builds off of the BIBFRAME Lite vocabulary. 
It is framework conformant to BIBFRAME and where possible, link-compatible with the 
US Library of Congress's BIBFRAME vocabulary, http://bibframe.org/. This draft starts 
with a mapping of the PREMIS Preservation Metadata Schema Version 2.3:

http://www.loc.gov/standards/premis/v2/premis-v2-3.xsd

This mapping will be updated to accomodate PREMIS Version 3.0 as soon as possible. 

BIBFRAME Preservation is expressed using the Versa data model, which also
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

You'll notice that BIBFRAME Preservation terms use a humpCase/HumpCase convention,
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
    * @base: http://bibfra.me/vocab/pres/
    * @property: http://bibfra.me/purl/versa/support
* title: BIBFRAME Preservation vocabulary
* @interpretations:
    * scope: @resource

<!---
Extend BIBFRAME Lite Classess
--->

# <http://bibfra.me/vocab/lite/Work>
* properties:  

# <http://bibfra.me/vocab/lite/Instance>
* properties: representation file bitstream

# <http://bibfra.me/vocab/lite/Authority>

# <http://bibfra.me/vocab/lite/Person>
* properties: 

# <http://bibfra.me/vocab/lite/Organization>
* properties: collectingInstitution

# <http://bibfra.me/vocab/lite/Meeting>
* properties: 

# <http://bibfra.me/vocab/lite/Topic>
* properties: 

# <http://bibfra.me/vocab/lite/Form>
* properties: 
    
# <http://bibfra.me/vocab/lite/Annotation>
* properties: accepts rejects
    
# <http://bibfra.me/vocab/lite/Event>
* properties: preservationEvent

<!---

Classes
-->


# 

* label: 
* refines: 
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# preservationEvent

* label: preservation event
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 


<!---

Properties

-->

# collectingInstitution

* label: collecting institution
* refines: http://bibfra.me/vocab/lite/Organization
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

<!---

(?+) would accepts/rejects work better in bibfra.me/vocab/relation?

-->

# accepts

* label: accepts
* refines:  http://bibfra.me/vocab/lite/Annotation
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# rejects

* label: rejects
* refines: http://bibfra.me/vocab/lite/Annotation
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# representation

* label: representation
* refines: http://bibfra.me/vocab/lite/Instance
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# file

* label: file
* refines: http://bibfra.me/vocab/lite/Instance
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# bitstream

* label: bitstream
* refines: http://bibfra.me/vocab/lite/Instance
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:


#

* label:
* refines:
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 




