---
layout: page
title: Data Access | The F# Software Foundation
headline: Data Access with F#
---

F# has a wide range of useful data import and access techniques available. Many F# books
and introductions cover some of these. 

The Type Provider feature of 
F# 3.0 brings simplicity to accessing both regular and irregular data, including traditional databases,
web-scale data and standard structured text formats like JSON, and XML.

[Try F#](http://tryfsharp.org/learn) has specific tutorials related to data access. 

### SQL Data Access

A wide range of high-quality libraries exist for SQL data access from F#. Some resources are listed below:

 * [The SqlDataConnection Type Provider](http://msdn.microsoft.com/en-us/library/hh361033.aspx) - For accessing SQL using F# 3.0 LINQ queries
 * [The SqlEntityConnection Type Provider](http://msdn.microsoft.com/en-us/library/hh361035.aspx) - For accessing SQL using F# 3.0 LINQ queries and Entity Framework
 * [ADO.NET](http://msdn.microsoft.com/en-us/library/h43ks021(v=VS.71).aspx) - A lower-level library for database access

### CSV, XML and JSON data

Some specific frameworks dedicated to simplifying document data  access are:

 * [FSharp.Data](http://tpetricek.github.io/FSharp.Data/) - The F# Data library (FSharp.Data.dll) implements everything you need to access data in your F# applications and scripts. It implements F# type providers for working with structured file formats (CSV, JSON and XML) and for accessing the WorldBank and Freebase data. It also includes helpers for parsing JSON files and for sending HTTP requests.
 * [Json.NET](http://json.codeplex.com/) - "Serialize All Things"

### Data Stores

The F# Type Provider machanism allows for the direct integration of scalable data stores into F# programming. Some specific examples are:

 * [Freebase](http://freeebase.com) - A type provider for Freebase is available in the [FSharp.Data](http://tpetricek.github.io/FSharp.Data/) library
 * [World Bank](http://worldbank.org) - A type provider for the World bank data sets is available in the [FSharp.Data](http://tpetricek.github.io/FSharp.Data/) library
