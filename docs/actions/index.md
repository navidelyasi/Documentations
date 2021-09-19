---
layout: default
title: Actions
nav_order: 4
has_children: true
permalink: /docs/actions
---
# Commonly used actions

## Array
[Count]():  Counts the number of elements in the list.

[Insert-At]():  Inserts the element in a given position. Commonly used with Iteration/for-each to extract data from a list of objects

[Sort](): Used to sort array elements in ascending order
Unique: Used to remove duplicate elements from the list

## Communication
[Http-Request]():  Most API calls used are HTTP requests.  Commonly used in conjunction with String/Join to prepare the URL by joining value from various sources.

## Conditional
[IF](): If condition is used in many logic scenarios from processing simple tasks, to automating complex workflows.

## Config
[Start-Timer]():  Used to start the timer based on a condition.

[Stop-Timer]():  Used to stop the timer based on a condition. Commonly used to start or stop the time after the flow or iteration is complete.

## Data
[Expression](): Used to apply code script (Elixir) for functions not supported with the built-in actions.

[Log](): Used to debug the solution.

[Set](): Used to apply data.

[Get-Variable](): Used often to get value from the Environment variable.

## Database
[Postgres](): Connector to Postgres database. MySQL is also a commonly used connector.

## DateTime
[Now](): Used to get the current time
Current-Unix-Time: Used to get current unix-time for easier time calculations

## File
[Read](): Used to read data from the file.

[Write](): Used to write data to the file.

## Flow
[Flow](): Used to group chain of actions into a reusable function

## Iteration
[Filter](): Lightest on compute. Commonly used to filter out elements from a large list of data.

[For-Each](): Used when extracting out certain values from the data. Does not change the original data.

[MAP](): Used to change the original data. Does not extract a certain value from the data

## Integer
[To-String](): Used to convert a number into a string

## JSON
[Decode](): Commonly used when working with HTTP Request body.  Data in the request body is normally a JSON string hence needs to be decoded into an object.

[Encode](): Commonly used when sending data over HTTP Response, writing to file, etc

## Organization
[Group]():  Commonly used to organize and group the actions. It is also convenient when moving a group of actions between flows.

## String
[Base-64-Encode](): Commonly used to encode ID and Password.

[Base-64-URL-Encode](): Commonly used to convert a string into a URL.

[Character-Decode](): Commonly used when working with foreign characters.

[Join]():  URL, query, system command, etc in most cases is a combination of value from many sources.  String/join is used to concatenate those values into a single string.

[Regex-Split](): Commonly used when working with CSV files to split the new line.

[Replace](): Commonly used for working with a timestamp. E.g. changing YYYY/MM/DD to YYYY-MM-DD by replacing / with - .

[Slice](): Commonly used when retrieving just the year (YYYY) from YYYYMMDD. Slice at position 4.

[Split-At](): Commonly used when splitting YYYYMMDD to make YYYY and MMDD from. Split at position 4.

[Split-With]():  Commonly used when splitting YYYY/MM/DD to make YYYY, MM, and DD. Split with character /.

[To-Integer](): Commonly used to convert string to an integer.

## Full list

{: .fs-6 .fw-300 }
