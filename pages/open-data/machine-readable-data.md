# Machine-readable data

In the context of working with data, **machine-readable does not simply mean openable by a computer**. For files or formats to be considered machine-readable, they should allow for **easy extraction, processing, and analysis of the data that they contain**. The most common application of this is with tabular data. A simple test for machine-readability is if you can automatically compute for the average of tabular data stored on the file. You can do this easily with spreadsheets but not so much with word documents, PDFs, or images.

Common examples of machine-readable formats for tabular data are:
- Comma-Separated Value files os CSV (.csv)
- Other Delimited Text Files (.tsv)
- Spreadsheet files (.ods, .xls, .xlsx)
- JavaScript Object Notation or JSON (.json)
- Databases

```yaml remark
type: success
text: Because of recent advancements in technology, the line between traditional machine-readable and non-machine-readable file formats for tabular data is slowly disappearing. There are now applications that make it possible to directly extract and process tabular data from PDFs and images albeit not as easily as it is with spreadsheets.
```

```yaml remark
type: warning
text: Machine-readable can have different meanings in other contexts. A file or format that's not normally considered machine-readable in one context may be considered machine-readable in another. For example, image files are not normally considered machine-readable if the purpose is to extract a table from the image but the same image may be considered as machine-readable for purposes of image analysis or pattern recognition. 
```

## Why is machine-readability important?

```yaml remark
type: primary
text: <b>Consider this scenario:</b><br>Juan and Pedro, <strong>persons of similar skill and capabilities</strong>, are both tasked with analysing the procurement activities of Procuring Entity A for the past 10 years.<br><ul><li>Juan is provided a PDF document containing the tables of A’s procurement activities.</li><li>Pedro was given the same dataset but in spreadsheet format.</li></ul><strong>Who do you think will be able to provide answers faster and more accurately, Juan or Pedro?</strong>
```

Having machine-readable data allows data users to focus on creating knowledge, providing insight, and building solutions with the data instead of spending a lot of time converting data from one format to another. If also facilitates reusability of data and replicability of results. **Machine-readability is a prerequisite to having open and reusable data.**

## Converting non-machine-readable into machine-readable
When working with data, it is often necessary to convert non-machine-readable files into machine-readable ones. This includes activities such as:
- Extracting a table from a PDF
- Getting a table from a webpage using web scraping tools
- Digitizing hard copy documents and extracting the data from them

This steps are usually done in the [get phase](../data-pipeline/get.md) of the [Data Pipeline](../data-pipeline/what-is-data-pipeline.html).

## Tidy data
The [tidy data principles](https://kiwidamien.github.io/what-is-tidy-data.html) state that for data to be tidy, it must be stored such that:
1. Each variable forms a column, and that column contains one "type" of data
2. Each observation forms a row
3. Each type of observational unit forms a table

There are multiple ways by which data can become untidy, [Hadley Wickham's paper on the subject matter](http://vita.had.co.nz/papers/tidy-data.pdf) identify these as:
1. Column headers contain values, rather than names
2. Multiple variables are stored in a single column
3. Variables are stored in both rows and columns
4. Multiple observational types are stored in a single table
5. A single observational unit is stored in multiple tables.

Ensuring that data is tidy will help you easily identify:
1. The types or categories of data points, with one data point per column. Each type of information is described across multiple observations. 
2. The individual observations, with one observation per row. An observation is a collection of data points made about a specific thing.  