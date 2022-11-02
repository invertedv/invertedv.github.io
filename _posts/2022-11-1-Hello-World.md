---
layout: post
title: Current Projects
---

These days I've been working on tools in Go for working with data using 
[ClickHouse](https://clickhouse.com/clickhouse) as the backend.

Here's what's been done since April of this year:

- [chutils](https://pkg.go.dev/github.com/invertedv/chutils) is a package to move data in and out of
ClickHouse. You can, for instance, point to a CSV, let the package determine the data types and then load
a table. Or, you can run a query and output the results to a new table.  You can also add new fields.
Finally, you can specify legal values and what to do if the value is outside that set or is null.

- [fannie](https://pkg.go.dev/github.com/invertedv/fannie) is an app for loading the data made available
from Fannie Mae into ClickHouse.  The data is housed as a single table with the monthly values being
nested arrays.

- The [freddie](https://pkg.go.dev/github.com/invertedv/freddie) app does the same but for the
Freddie Mac data.

- [toch](https://pkg.go.dev/github.com/invertedv/toch) is an app for moving data from the web or files
into ClickHouse.  

- [fred2ch](https://pkg.go.dev/github.com/invertedv/fred2ch) is an app for moving data from the St. Louis Fed's Fred II database to ClickHouse.

- [sampler](https://pkg.go.dev/github.com/invertedv/sampler) is a package that creates a stratified sample
from a source ClickHouse query.  The output sample is saved to ClickHouse as is a table of the strats and
counts.

- [seafan](https://pkg.go.dev/github.com/invertedv/seafan) is a package of model-building tools for
DNN models.  It has data pipelines, model-specification methods, diagnostics and more.  The fitting
algorithm uses the awesome [gorgonia](https://pkg.go.dev/gorgonia.org/gorgonia@v0.9.17#section-readme) 
package.