jsonschema-schema.org
=====================

[schema.org](http://schema.org/) glossary in [JSON Schema](http://json-schema.org/) for convenience of use from codes.

In example, [Thing](http://schema.org/Thing) format is represented in JSON Schema as follows.

```json
{
  "$schema": "http://json-schema.org/draft-04/schema#",
  "id": "http://schema.org/Thing",
  "required": false,
  "title": "Thing",
  "name": "Thing",
  "description": "The most generic type of item.",
  "type": "object",
  "properties": {
    "additionalType": {
      "id": "http://schema.org/additionalType",
      "required": false,
      "title": "additionalType",
      "description": "An additional type for the item, typically used for adding more specific types from external vocabularies in microdata syntax. This is a relationship between something and a class that the thing is in. In RDFa syntax, it is better to use the native RDFa syntax - the 'typeof' attribute - for multiple types. Schema.org tools may have only weaker understanding of extra types, in particular those defined externally.",
      "type": "string"
    },
    "alternateName": {
      "id": "http://schema.org/alternateName",
      "required": false,
      "title": "alternateName",
      "description": "An alias for the item.",
      "type": "string"
    },
    "description": {
      "id": "http://schema.org/description",
      "required": false,
      "title": "description",
      "description": "A short description of the item.",
      "type": "string"
    },
    "image": {
      "id": "http://schema.org/image",
      "required": false,
      "title": "image",
      "description": "An image of the item. This can be a URL or a fully described ImageObject.",
      "type": "string"
    },
    "name": {
      "id": "http://schema.org/name",
      "required": false,
      "title": "name",
      "description": "The name of the item.",
      "type": "string"
    },
    "potentialAction": {
      "id": "http://schema.org/potentialAction",
      "required": false,
      "title": "potentialAction",
      "description": "Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role.",
      "type": "object",
      "properties": {
        "potentialAction": {
          "$ref": "Action.json#/properties"
        }
      }
    },
    "sameAs": {
      "id": "http://schema.org/sameAs",
      "required": false,
      "title": "sameAs",
      "description": "URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Freebase page, or official website.",
      "type": "string"
    },
    "url": {
      "id": "http://schema.org/url",
      "required": false,
      "title": "url",
      "description": "URL of the item.",
      "type": "string"
    }
  }
}
```

Learn JSON Schema
---

There is a great e-Book! [Understanding JSON Schema](http://spacetelescope.github.io/understanding-json-schema/index.html)

Build Latest One
---

https://github.com/kaiinui/build-jsonschema-schema.org provides build tool.

LICENSE
---

The license conforms to [schema.org's license](http://schema.org/docs/terms.html) - [Creative Commons Attribution-ShareAlike License (version 3.0)](http://creativecommons.org/licenses/by-sa/3.0/)
