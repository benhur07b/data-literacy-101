# Find
> Where is the data located and is it accessible?

This step entails knowing **where to look** for your data, finding it, and knowing how accessible it is. This is a step of **varying difficulty** depending on how well you defined your data problem.

Finding data also depends on your **creativity and critical thinking**. When data seems hard to find, you can consider looking at **proxy indicators**—an indirect measure or sign that indicates a phenomenon in the absence of a direct measure or sign.

## Things to consider
### Asking the right questions
It is impossible for a single person to know where to find all the data that you need which is why experience, contextual knowledge, and having contacts in the relevant fields are key assets that will help you find the right dataset for your project. 

Be mindful of the fact that several sources may maintain similar datasets where one dataset is a better fit for some projects than others. Your task is to understand the precise data needs of your project in order to compare it with all the available data that you find. This step is important as it may lead your team to review the scope or research question of the project.


When looking for data, you can:
- Ask if there is a national government agency mandated to collect the data.
- Ask if there are organizations or individuals who are working or have worked with the data.
- Ask if there are any other datasets that can serve as indicators for the data needed?
- Use online search engines (utilizing advanced search capabilities makes searching easier).
- Use libraries and museums.


### Data sources
There are a lot of tools, techniques, and data sources that can help you in finding data both online and offline. These include:
- Data portals
- Social networking sites
- [Google advanced search operators](https://developers.google.com/search/docs/advanced/debug/search-operators/overview)
- Google Dataset Search 
- FOI requests
- Libraries and librarians
- Museums and curators

```yaml remark
type: primary
text: What other sources can you think of?
```

### Understanding data formats
Different types of digital files use different structures to hold information. For example, a text file is structured differently than an image file, which is structured differently than a web page. At the same time, most computer applications can only open a few file types since they are programmed to work only with specific structures—i.e. a word processor cannot open a spreadsheet file. **It is important that you know about different file formats and how they relate to the data that you require so that you can better plan a strategy on how to [get the data](get.html)**.

Some of the most common file formats/file extensions that you might encounter when working with data include:
- **.txt** - TXT is the extension for basic text files. It is not a structured data format per se, but it is possible to write data in a text file and have the right software recognize the structure despite the .txt extension such as in **delimited text files** (see CSV/TSV below).

- **.csv/tsv** - CSV stands for Comma Separated Value and is used for storing tabular data: data arranged in rows and columns. An alternative is the TSV file format which uses tabs instead of commas to separate the values. Both of them are simply **text arranged in a structured way** The character used to separate values in the file (e.g. comma for CSV and tab for TSV) is known as the delimiter, hence the general name given to these kinds of files—delimited text files. The .csv or .tsv extension indicates to the software how to read the file but many applications can automatically detect the tabular structure in delimited text files even without the .csv or .tsv extension.

```yaml remark
type: success
text: CSV is probably the most preferred file format for sharing tabular data.  It is an open standard which means that you don't need proprietary or specialized software to open it.
```

- **.xls/.xlsx** - proprietary formats used by Microsoft Office to store its spreadsheets. Spreadsheets store tabular data similarly to CSV files but they also include information that is not purely data (e.g. the formulas used to compute cell values) and can store multiple tables in one file. As a consequence, spreadsheets are usually heavier (in terms of file size and the computing power needed to open them) than CSVs. Additionally, being a proprietary format might make .XLS and .XLSX less suitable for data sharing even if they have widespread use because of people's familiarity with Excel.

- **.ods** - an open file format for spreadsheets developed and maintained as part of the Open Document Format for Office Applications (ODF). It is widely used in both free and open source office applications (LibreOffice, ONLYOFFICE) as well as propietary ones (MS Office). Being an open format means that there is no need to purchase a proprietary application in order to open and use it.

- **.doc/.docx** - proprietary formats used by Microsoft Office to store word documents. They store more information (e.g. text formatting, images, links) than simple text files which makes them heavier to use. Similar to .XLS/.XLSX, they may be less suitable for data sharing even if they have widespread use because of people's familiarity with Word.

- **.odt** - an open file format for word documents developed and maintained as part of the Open Document Format for Office Applications (ODF).

- **JSON** - JavaScript Object Notation is designed to be lightweight, web-native, easy to read by programming languages, and easy to share through APIs. While JSON is an international standard like CSV, they store different types of data structures: CSV is designed for tabular data while JSON structures its data in a tree-like structure. The [Open Contracting Data Standard](https://standard.open-contracting.org/latest/en/) uses a JSON schema as its data model. 

- **GeoJSON** - JSON with accompanying location information—i.e. coordinates (latitude and longitude), vector data model (point, line, polygon). It is useful for working with geospatial information on the web.

- **shapefile** - a proprietary format for storing spatial vector data for ESRI products. Similar to .XLS, it is a well-known and widely-used format even if it has [limitations](https://bnhr.xyz/2018/12/12/i-choose-geopackage.html).

- **geopackage** - an open format by the Open Geospatial Consortium for storing spatial data (both vector and raster) which has [can overcome the limitations of shapefiles](https://bnhr.xyz/2018/12/12/i-choose-geopackage.html).

```yaml remark
type: success
text: <strong>Tabular vs Tree structure</strong><br>When is each structure most appropriate? As a new data practitioner, the easiest data to deal with would be those that are stored in tabular format. This means that you know in advance how many columns/fields your dataset should have and that all data fit into these columns neatly.<br><br>But what if you can’t predict some part of your data? Take a list of public procurement bids. You may want to include, at minimum, the project name, the approved budget of contract, the procuring entity, the bid amount, and the bidders. But some projecs will have 2 bidders and others may have 30. To store this in a tabular format, you would have to compromise the quality or structure of your dataset&#58;<ul><li>Either you store all bidders in one column, which will make analysis harder</li><li>Or you add a lot of columns/fields in order to write one bidder per column and hope that the number of bidders will never go over the number of columns you set. You may end up with a dataset full of empty values/cells and a cumbersome amount of columns (which may or may not be needed).</li></ul>This is when a format like JSON that has a tree structure might be the better option. The tree format can associate an arbitrary number of values to each node/field. If the number of bidders from your first project differs from your second one, this will just change the number of branches linked to each node/field and not the number of nodes/fields in the data. <br><br>Beyond their differences, <strong>both CSV and JSON are international open standards that are widely adopted, designed to be readable by humans without a need for software, and should be preferred over their closed alternatives</strong>.
```

## Common issues

### Settling for a poor quality dataset
When looking for data that you need, it is **not uncommon for you to find multiple datasets and sources** pertaining to the same data. Try to avoid the temptation to settle on the first dataset you find and adjust the project based on that without investigating further if there are better options. 

Sometimes it may be **more useful to create the needed dataset out of several quality datasets** rather than settling for the obvious choice. 
