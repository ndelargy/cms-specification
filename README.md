#Parrot CMS Specification

Document to define the CMS specification and it's components. 

**Table of Contents**
=======================
1. [API](#api)
  1. [Resources](#resources)
    1. [Owner](#owner)
    2. [Interface](#interfaces)
    3. [Interface Type](#interface-type)
    4. [Page](#page)
    5. [Content Block](#content-block)
    6. [Content](#content)
    7. [Author](#author)
  2. [Authentication](#authentication)
    1. OAUTH 2.0
2. [Interfaces](#Interfaces)
  1. [Website](#website)
  2. [Mobile/Tablet Application](#mobiletablet-application)
  2. [Admin Dashboard](#admin-dashboard)

# API
## Resources 
### Owner
An Owner Resource is an authoritive entity which owns Resources associated under it. [Interfaces](#interface), [Content Blocks](#content-block) and [Content](#content) etc cannot be associated with more than one Owner and will not be visible by other parties. 

[Interface Types](#interface-type) and [Content Types](#content-type) will also not be shared across Owners, however there will be a pre-defined collection of types for each that can be used to define Owner specific types.

### Interface
Interface Resources describe the relationship and association of Page, Content Block and Content Resources with one another.

e.g. A [Website](#website) Interface may share [Page](#page) Resources and it's associated [Content Blocks](#content-block) but have different [Content](#content) Resources for each; this allows an [Author](#author) to tailor their content for a particular [Interface](#Interface).

An Interface Resource must as a minimum requirement define a type and provide a name/alias to associate with that type. e.g. Type: Website, Alias: www.mysite.com

["There can only be one"](https://www.google.co.uk/search?q=there+can+only+be+one&oq=there+can+only+be+one) [Interface Type Resource](#interface-type) per [Owner](#owner) and these will be selected from a pre-defined collection.
### Interface Type
### Page
### Content Block
#### Content Block Type
### Content
### Author
##Authentication
# Interfaces
## Website
## Mobile/Tablet Application
## Admin Dashboard
