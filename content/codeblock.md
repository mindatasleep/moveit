---
title: "Syntax Highlighting"
metaTitle: "Syntax Highlighting is the meta title tag for this page"
metaDescription: "This is the meta description for this page"
---

The following is a code block with JavaScript language syntax highlighting.

```javascript
import React from 'react';
```

Supports multiple languages.

The following is a code block with diff. Lines with `+` highlighted in green shade indicating an addition. Lines with `-` highlighted in red shade indicating a deletion.

```javascript
- const data = ['1','2'];
+ const data = [1,2];
```

## Live Editing example

```javascript react-live=true
<button className={'btn btn-default'}>Change my text</button>
```

## Ejemplo

```sql
-- a circle within a circle
SELECT ST_Within(smallc,smallc) As smallinsmall,
	ST_Within(smallc, bigc) As smallinbig,
	ST_Within(bigc,smallc) As biginsmall,
	ST_Within(ST_Union(smallc, bigc), bigc) as unioninbig,
	ST_Within(bigc, ST_Union(smallc, bigc)) as biginunion,
	ST_Equals(bigc, ST_Union(smallc, bigc)) as bigisunion
FROM
(
SELECT ST_Buffer(ST_GeomFromText('POINT(50 50)'), 20) As smallc,
	ST_Buffer(ST_GeomFromText('POINT(50 50)'), 40) As bigc) As foo;
```
