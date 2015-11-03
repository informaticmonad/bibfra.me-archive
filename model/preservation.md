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
* properties: handle

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
    
# <http://bibfra.me/vocab/lite/Annotation>
* properties: accepts rejects inhibitor
    
# <http://bibfra.me/vocab/lite/Event>
* properties: outcome

<!---

Comments: 
    
    Premis terms already in BF Lite:
    * http://bibfra.me/vocab/lite/Organization
    * http://bibfra.me/vocab/lite/Person
    * http://bibfra.me/view/lite/link/
    * http://bibfra.me/vocab/lite/copyright
    * http://bibfra.me/vocab/lite/CopyrightEvent (copyrighted)
    * 
    
    Premis Elements alread in BF Lite + Relation:
    * http://bibfra.me/vocab/relation/isPartOf
      * Does a http://id.loc.gov/vocabulary/preservation/relationshipSubType/isp synonym need to be made on the Relation layer?
    * http://bibfra.me/vocab/relation/hasPart
      * h " " synonym for id.loc.gov/vocabulary/preservation/relationshipSubType/hsp in the Relation layer
    
-->
   
<!---
    
Versa template: 
    
    # 

    * label: 
    * refines: 
    * synonyms: 
    * description: 
    * value: 
    * properties: 
    * scope: <http://bibfra.me/vocab/pres/>
    * remark:

-->

<!---

Below are added terms outside of the scope of LC's preservation vocabs and BF Lite, or elements defined in a new way unique to the BF Lite + Preservation layer. Some options are possibly better suited for the BF Lite + Annotation layer.  
    
-->

## CollectingInstitution

* label: collecting institution
* refines: http://bibfra.me/vocab/lite/Organization
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

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

<!---

Below I'm experimenting with defining the inhibitor target collection relationships as refinements of BF Lite + Annotations. See: http://id.loc.gov/vocabulary/preservation/inhibitorTarget/collection_PREMIS.html

-->

# inhibitor

* label: Print Function
* refines: http://bibfra.me/vocab/lite/annotator
* synonyms: 
* description: An agent that inhibits someone or something.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# AllContent

* label: AllContent
* refines: http://bibfra.me/vocab/lite/Annotation
* synonyms: 
* description: Inhibitor prohibits use of all content.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# PlayFunction

* label: Play Function
* refines: http://bibfra.me/vocab/lite/Annotation
* synonyms: 
* description: Inhibitor prohibits function of play.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# PrintFunction

* label: Print Function
* refines: http://bibfra.me/vocab/lite/Annotation
* synonyms: 
* description: Inhibitor prohibits function of print.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

<!---

Deaccession, Use, and Decompression are already Event Types in PREMIS. I refined Event when defining them here. These actions should be Events too:

-->

# Migrate

* label: Migrate
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/actionsGranted/mig
* description: The process of removing an object from the inventory of a repository.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Delete

* label: Delete
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/dea
* description: The process of removing an object from a repository.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Disseminate

* label: Disseminate
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/dis
* description: Create a copy or version for use outside of the preservation repository.
* value: 	
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Modify

* label: Modify
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/mod
* description: Make a version different in content.
* value: 	
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Replicate

* label: Replicate
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/rep
* description: Make an exact copy. 
* value: 	
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

<!---

In LC's preservation vocabularies software is defined as an Agent. Totally understandable. But then there is Software Types. Instead of types I think they should be refinements of Software. The wouldn't be 1:1 synonyms but I'm reapplying the definitions. 
    
-->


# OperatingSystem

* label: Operating System
* refines: http://bibfra.me/vocab/lite/Agent
* synonyms: http://id.loc.gov/vocabulary/preservation/softwareType/ops
* description: Software that supports application execution, process scheduling, memory management, file systems, etc.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# Ancillary

* label: Ancillary
* refines: http://bibfra.me/vocab/lite/Agent
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Driver

* label: Driver
* refines: http://bibfra.me/vocab/lite/Agent
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Renderer

* label: Renderer
* refines: http://bibfra.me/vocab/lite/Agent
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:


<!---

End of terms with definitions unique to the BF Lite + Preservation layer, and possible BF Lite + Annotation candidates. Below are PREMIS mappings based on http://id.loc.gov/vocabulary/preservation. 
    
-->

<!---
    
    As with Signature Method (defined further down below) I refined Concept with Cryptographic Hash Functions because BF Lite does not have a SKOS:ConceptScheme equivalent. However instead of refining BF Lite control code like I did with the properties of Signature Method, I refined Concept for the properties of CryptographicHashFunctions. This at least provides 1:1 synonym relationships for the properties, but I don't think CryptographicHashFunctions is a 1:1 synonym because LC's is an instance of SKOS:ConceptScheme and here I'm refining Concept. I can imagine ConceptScheme being equated with http://bibfra.me/view/links/lite/Category/ and the properties of CryptographicHashFunctions and SignatureMethod being contained in those controlled vocabularies. 
    
-->

# CryptographicHashFunctions

* label: Cryptographic Hash Functions
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions
* description: Cryptographic hash functions are transformations that takes an input and returns a fixed-size string, which is called the hash value. Hash functions with this property are used for a variety of computational purposes, including cryptography. The hash value is a concise representation of the message or document from which it was computed. Cryptographic hash functions are used to do message integrity checks and digital signatures in various information security applications, such as authentication and message integrity. They may also be referred to as message digest algorithms or checksum algorithms.
* value: 
* properties: adler-32 crc32 haval md2 md5 mnp sha-1 sha-256 sha-384 sha-512 tiger unknown whirlpool ripemd-160
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# PreservationEvent

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

## adler-32

* label: Adler-32
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/adler
* description: Adler-32 is a checksum algorithm which was invented by Mark Adler. Compared to a cyclic redundancy check of the same length it trades reliability for speed. Compared to its original form (Fletcher-16), Adler-32 is more reliable than Fletcher-16. However, Adler-32 is slightly less reliable than Fletcher-32.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

## crc32

* label: CRC32
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/crc32
* description: A cyclic redundancy check (CRC) 32 is a type of function that takes as input a data stream of any length and produces as output a value of a certain fixed size. The term CRC is often used to denote either the function or the function's output. A CRC can be used as a checksum to detect accidental alteration of data during transmission or storage.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

## haval 

* label: HAVAL
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/haval
* description: HAVAL is a cryptographic hash function. HAVAL can produce hashes in lengths of 128 bits, 160 bits, 192 bits, 224 bits, and 256 bits. HAVAL also allows users to specify the number of rounds (3, 4, or 5) to be used to generate the hash.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## md2

* label: MD2
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/md2
* description: In cryptography, MD2 (MD2 Message-Digest Algorithm) is a cryptographic hash function with a 128-bit hash value. As an Internet standard (RFC 1319), MD2 is commonly used to check the integrity of files. An MD2 hash is typically expressed as a 32-character hexadecimal number.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## md5

* label: MD5
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/md5
* description: In cryptography, MD5 (Message-Digest algorithm 5) is a widely used cryptographic hash function with a 128-bit hash value. As an Internet standard (RFC 1321), MD5 has been employed in a wide variety of security applications, and is also commonly used to check the integrity of files. An MD5 hash is typically expressed as a 32-character hexadecimal number.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## mnp

* label: MNP
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/mnp
* description: The MNP (Microcom Networking Protocol) family of error-correcting protocols were commonly used on early high-speed (2400 bit/s and higher) modems. Originally developed for use on Microcom's own family of modems, the protocol was later openly licensed and used by most of the modem industry, notably the "big three", Telebit, USRobotics and Hayes. MNP was later supplanted by v.42bis, which was used almost universally on the first v.32bis modems in the early 1990s.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## ripemd-160
* label: RIPEMD-160
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/mnp
* description: RACE Integrity Primitives Evaluation Message Digest is a 160-bit message digest algorithm (and cryptographic hash function) developed in Leuven (Belgium) by Hans Dobbertin, Antoon Bosselaers and Bart Preneel at the COSIC research group at the Katholieke Universiteit Leuven, and first published in 1996.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:


<!---

In LC's preservation vocab the SHA Algrothms are defined as related. Not sure if that is nessisary here. They are all properties of CryptographicHashFunctions.

-->


## sha-1

* label: SHA-1
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/sha1
* description: Secure Hash Algroithm 1. SHA stands for Secure Hash Algorithm. Hash algorithms compute a fixed-length digital representation (known as a message digest) of an input data sequence (the message) of any length.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## sha-256

* label: SHA-256
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/sha256
* description: Secure Hash Algroithm 256. SHA stands for Secure Hash Algorithm. Hash algorithms compute a fixed-length digital representation (known as a message digest) of an input data sequence (the message) of any length.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## sha-384

* label: SHA-384
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/sha384
* description: Secure Hash Algorithm 384. SHA stands for Secure Hash Algorithm. Hash algorithms compute a fixed-length digital representation (known as a message digest) of an input data sequence (the message) of any length.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## sha-512

* label: SHA-512
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/sha512
* description: Secure Hash Algorithm 512. SHA stands for Secure Hash Algorithm. Hash algorithms compute a fixed-length digital representation (known as a message digest) of an input data sequence (the message) of any length.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

## tiger

* label: TIGER
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/tiger
* description: Tiger is a cryptographic hash function designed by Ross Anderson and Eli Biham in 1995 for efficiency on 64-bit platforms. The size of a Tiger hash value is 192 bits. Truncated versions (known as Tiger/128 and Tiger/160) can be used for compatibility with protocols assuming a particular hash size.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

## unknownHash

* label: unknown hash
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/unk
* description: Unknown hash indicates that a hash function was used but which it is cannot be adequately determined.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

## whirlpool

* label: WHIRLPOOL
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/cryptographicHashFunctions/whirl
* description: Whirlpool (sometimes styled WHIRLPOOL) is a cryptographic hash function designed by Vincent Rijmen (co-creator of the Advanced Encryption Standard) and Paulo S. L. M. Barreto. The hash has been recommended by the NESSIE project. It has also been adopted by the International Organization for Standardization (ISO) and the International Electrotechnical Commission (IEC) as part of the joint ISO/IEC 10118-3 international standard.
* value: CryptographicHashFunctions
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# Creation

* label: creation
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/cre
* description: The act of creating a new object.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## outcome

* label: outcome
* refines: http://bibfra.me/vocab/lite/related
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/out
* description: The object in relation to the described event is the outcome of that event.
* value: Event 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

## handle

* label: handle
* refines: http://bibfra.me/vocab/lite/authoritylink
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/out
* description: Unique and persistent identifiers used in the Handle System. A handle is a character string that consists of a naming authority followed by a unique local name under the naming authority.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# Deaccession

* label: Deaccession
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/dea.html
* description: The process of removing an object from the inventory of a repository.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

<!---

Not sure if the refinements of Instance below are 1:1 synonyms.

-->

# bitstream

* label: bitstream
* refines: http://bibfra.me/vocab/lite/Instance
* synonyms: http://id.loc.gov/vocabulary/preservation/objectCategory/bit
* description: Contiguous or non-contiguous data within a file that has meaningful properties for preservation purposes.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

# SignatureEncoding

* label: singatureEncoding
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureEncoding/
* description: The type of encoding used in a digital signature.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# Ds:CryptoBinary

* label: ds:CryptoBinary
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureEncoding/dscb
* description: An encoding type for representing arbitrary-length integers (e.g. "bignums") in XML as octet strings. 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 


# Base64

* label: base64
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureEncoding/base64
* description: A group of similar encoding schemes that represent binary data in an ASCII string format by translating it into a radix-64 representation.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# Base64

* label: base64
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureEncoding/base64
* description: An encoding type for representing arbitrary-length integers (e.g. "bignums") in XML as octet strings. 
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

# 

* label: 
* refines: 
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



#

* label:
* refines:
* synonyms: 
* description: 
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

Blowfish
CRC32
DFS

## dsa-sha1

* label: DSA-SHA1
* refines: http://bibfra.me/vocab/lite/controlCode
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureMethod/dsa-sha1
* description: Digital Signature Algorithm (DSA) is an algorithm developed by the United States Federal Government as a standard for digital signatures.
* value: SignatureMethod
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

EXT3
MNP
NTFS
PGP
TSM
ancillary
authorizer
base64
byteOffset
capability
capture
compression
contact
creation
cryptobinary
deaccession
decompression
decryption
delete
deletion
derivation
digitalSignatureValidation
disseminate
driver
edit
executingProgram
fixityCheck
grantor
handle
hardDisk

# Hardware

* label: hardware
* refines: http://bibfra.me/vocab/lite/Agent
* synonyms: http://id.loc.gov/vocabulary/preservation/agentType/sof  
* description: Program or programs used to direct the operation of a computer, as well as documentation giving instructions on how to use them.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 



hasRoot
hasSibling
hasSource
implimenter
includes
ingestion
inputOutputDevice
intention
isIncludedIn
isSourceOf
knownToWork
license
magneticTape
md5
memory
messageDigestCalculation
migrate
migration
minimum
modify
normalization
operating system
other
outcome
passwordProtection
playFunction
print function
processor
public domain
recommended
render
renderer
replicate
replication
representation
requirement
rightsholder
ripemd-160

## rsa-sha1

* label: RSA-SHA1
* refines: http://bibfra.me/vocab/lite/controlCode>
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureMethod/rsa-sha1
* description: Algorithm for public-key cryptography that is based on the presumed difficulty of factoring large integers.
* value: SignatureMethod
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

<!---

http://id.loc.gov/vocabulary/preservation/signatureMethod/rsa-sha1 is an instance of SKOS:ConceptScheme, but here I've refined Concept. I think it works but the 1:1 synonym may not be valid if BF Lite + Pres refines BF Lite Concept and LC refines SKOS:ConceptScheme. That might also mean LC's dsa-sha1 and rsa-sha1 might not be 1:1 synonyms but I think refining Concept works well here - it comes with appropriate properties.  Also I made dsa-sha1 and rsa-sha refinements of control code (alphanumberic literal identifier, works well, but again not sure if they're 1:1 synonyms).

-->


# Signature Method

* label: RSA-SHA1
* refines: http://bibfra.me/vocab/lite/Concept
* synonyms: http://id.loc.gov/vocabulary/preservation/signatureMethod/rsa-sha1
* description: Designation of the encryption and hash algorithms used for signature generation.
* value: 
* properties: rsa-sha1 dsa-sha1
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

# Software

* label: software
* refines: http://bibfra.me/vocab/lite/Agent
* synonyms: http://id.loc.gov/vocabulary/preservation/agentType/sof  
* description: Program or programs used to direct the operation of a computer, as well as documentation giving instructions on how to use them.
* value: 
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark: 

source
specification
statute
storageDevice
structural
unknown
unspecified

# Use

* label: Use
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/use
* description: Read without copying or modifying (e.g., to validate a file or run a program).
* value: 	
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:


# Decompression

* label: Decompression
* refines: http://bibfra.me/vocab/lite/Event
* synonyms: http://id.loc.gov/vocabulary/preservation/eventType/dec
* description: The process of reversing the effects of compression.
* value: 	
* properties: 
* scope: <http://bibfra.me/vocab/pres/>
* remark:

validation
validationProfile
validator
virusCheck


