# json-to-pretty-yaml

> A node module to convert JSON to YAML.

## Installation

`npm install --save json-to-pretty-yaml`

## Usage

#### Code

```
const YAML = require('json-to-pretty-yaml');

const json = {
  a: 1,
  b: "yes",
  c: true,
  d: undefined,
  e: [
    1,
    2,
    {
      f: 'cool'
    }
  ]
}

const yaml = YAML.stringify(json);
console.log(yaml);
```

#### Output

```
a: 1
b: "yes"
c: true
e:
  - f: "cool"
    g: "new"
  - h: "free"
    i: "soon"
```
