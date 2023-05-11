# Malloy Design Patterns

To run these examples
* Log into Github
* press `.`  (the period key) to run vscode
* Install the Malloy Extension when prompted (or manually)

## Working with Nested Data
Malloy natively understands how to work with tables that have nested structs 
and arrays (including raw JSON) and makes easy to query and transform. 

[Nested Data](nested_data.malloynb)

## Sessionization
Take list of individual flights and map/reduce into individual aircraft sessions per day.  Display their routes for each day on a map.  Classic Map/Reduce.

[Flight Route Sessinization](flight_routes.malloynb)

## Automatic Historgrams

When drawing an histogram, you need to figure out a proper bin size to group the data.  This pattern dyamically computes bin sizing.  The binning automatically adusts with in filtered and nesting situations.

[Automatic Historgrams](auto_bin.malloynb)

## Deduping Rows of Data (or basing a query on SQL)

Sometime data comes in with duplicates.  We can base a query on a SQL Query to remove duplicates

[Dedup Rows](dedup_rows.malloynb)

## Querying Data directly from a Web API

Using DuckDB wwe can query from Web API endpoints.  This example pulls from the github and runs some transformation queries against the results

[HTTP API Queries](api_json.malloynb)

## Indexing the entire source graph
Malloy has a special 'index' operator that produces a result that contains all the dimensional values in a graph weighed by whatever measure 
you think is important.  The index can be built by reading the whole graph or sampling a subset of records.  The index is useful 
in suggesting filters and for basic understanding of a data set and perhaps informing an LLM.

[Malloy Dimensional Indexes](index.malloynb)

