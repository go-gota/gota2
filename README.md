# Gota: DataFrames, Series and Data Wrangling for Go

Meet us on Slack: Slack: [gophers.slack.com](https://gophers.slack.com) #go-gota ([invite](https://gophersinvite.herokuapp.com/))

---

Gota2 is a more typesafe version of Gota. Gota has limitations, because it's difficult to build a 1:1 implementation of an untyped API in a typed language. This led to bloated, hard to maintain code. Gota2 uses Go 1.18 with type parameters to support arbitrary data types. This causes a big and hard breaking change with no simple upgrade path. Onn the other hand, the new code is simpler and easier to maintain and extend.

---

This is an implementation of DataFrames, Series and data wrangling
methods for the Go programming language. The API is still in flux so *use at your own risk*.

## DataFrame

The term DataFrame typically refers to a tabular dataset that can be
viewed as a two dimensional table. Often the columns of this dataset
refers to a list of features, while the rows represent a number of
measurements. As the data on the real world is not perfect, DataFrame
supports non measurements or NaN elements.

Common examples of DataFrames can be found on Excel sheets, CSV files
or SQL database tables, but this data can come on a variety of other
formats, like a collection of JSON objects or XML files.

The utility of DataFrames resides on the ability to subset them, merge
them, summarize the data for individual features or apply functions to
entire rows or columns, all while keeping column type integrity.

## Series

Series are essentially vectors of elements of the same type with
support for missing values. Series are the building blocks for
DataFrame columns.

## License

Licensed under the Apache License, Version 2.0 (the "License"); you
may not use this file except in compliance with the License.  You may
obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
implied. See the License for the specific language governing
permissions and limitations under the License.
