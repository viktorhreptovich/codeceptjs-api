Clicking [this link](#1.1-My-First-Header) will scroll

# API Testing with codeceptjs


sdafasdf

sadfasdf

asdfasdf

sdafasdf

sadfasdf

asdfasdf

sdafasdf

sadfasdf

asdfasdf

sdafasdf

sadfasdf

asdfasdf

sdafasdf

sadfasdf

asdfasdf

***
# Contract
### Generate json schema

https://www.jsonschema.net/home

1. Setup Settings:
    - Version: "Draft-04"
    - Keyword Visibility: <span style="color:red">required</span>: "title", "type", "additionalItems", "uniqueItems", "
      required"
    - Array Validation: "First (single schema)"
    - Indentifier Type: "JSON Pointer Fragment"
    - Absolute URI: your URI
    - Objects: [x] Require properties
    - Arrays: [x] additionalItems [x] uniqueItems
    - Numeric: [x] JSON types only

![](readme/jsonshema.jpg)
2. Insert your json, check it is valid and press "SUBMIT". Json schema will be generated. 
3. Copy generated schema to clipboard and create <json_shema>.json file.
### Convert json schema to joi   

1. Install a utility to convert JSON schema (draft 4) to Joi validation schema
https://www.npmjs.com/package/json-schema-to-joi
2. Run command for generate joi validation schema:
```
> json2joi --input <json_shema>.json --output <contract_name>.js
```
3. Replace in your <contract_name>.js
```javascript
import * as Joi from '@hapi/joi';

export const theRootSchemaJoiSchema = Joi.object()
```
   to
```javascript
const Joi = require('joi');

module.exports.<contract_name> = Joi.object()
```
***
# 1.1 My First Header
