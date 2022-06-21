# Clean
> Just because data is dirty does not mean it's garbage.

There is a common saying among people who work regularly with data that "80% of the time spent working with data is spent cleaning it" and indeed, it is often an arduous task that is not only time-consuming but can also be error prone. The CLEAN step of the Data Pipeline works as a group with the VERIFY and ANALYSE steps—while simple datasets may only need to go through VERIFY, CLEAN and ANALYSE once, more complex datasets will see you go back and forth between the three. Specifically, you may find yourself:

- cleaning the dataset a bit to be able to verify its content
- going back to the verify step after finding something strange during the analysis
- doing some basic analysis steps as part of the verification process 

```yaml remark
type: success
text: <strong>Pristine data is very rare. Most of the time, the data you get will contain problems that you have to clean.</strong>
```

## Things to consider
### Goals of data cleaning
- create a consistent, human understandable, machine readable dataset
- prepare the data for a specific analysis or visualization you want to use the data for

### Data cleaning steps
Data cleaning can be broken down into three activities:

**1. Data tidying** is the process of cleaning the structure of the data without touching its content and following the princples of [tidy data](../open-data/machine-readable-data.html#tidy-data). 

**2. Data editing** is the process of modifying the content of the data to prepare it for your analysis. This involves correcting problems with the values stored in the dataset.

**3. Data consolidation** is the process of adding complementary data to your main dataset. This step provides an this is an opportunity to complement or extend the dataset that you have collected, verified and cleaned. The goal may be to produce a more complete analysis thanks to the addition of a new variable, or to simply consolidate in one dataset all the data that you will need to answer all your research questions.

```yaml remark
type: warning
text: <strong>Avoid deleting or overwriting the data in your original dataset</strong>. A better approach is to make copies of the data for each step of the data cleaning process or to utilize version control systems. 
```

```yaml remark
type: warning
text: <strong>Do not take a shortcut with data consolidation</strong>. The best practice is for you to go through the DEFINE, FIND, GET, VERIFY and CLEAN steps again with a new dataset before merging it with your main data. 
```

### Types of problems you might encounter
There are two general kinds of problems with the data that you might encounter when cleaning it:

**1. Formatting problems** - problems related to HOW the dataset is structured. These are usually resolved in the data tidying step.

**2. Content problems** - problems related to WHAT is written or stored in the dataset. These are usually resolved in the data editing step.

Examples of formatting problems include:

| **Type of problem** | **Problem**                                          | **Example**                                                                                                                                                                                                                                                                                                                                    | **Suggested solution**                 |
|---------------------|------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------|
| Formatting problem  | A single data point is stored in a multiple columns. | Address is saved as multiple columns of BARANGAY, MUNICIPALITY, and PROVINCE but you need it to be a single string                                                                                                                                                                                                                             | Concatenate values into a single cell  |
| Formatting problem  | Separate data points are stored in a single column.  | Address is saved as a single string of <BARANGAY>, <MUNICIPALITY> , <PROVINCE> but you need to summarize data based on BARANGAY for your analysis.                                                                                                                                                                                             | Split the column into several columns  |
| Formatting problem  | Multi-line or merged headers                         | Population data divided by age and sex where one row is used for age categories and another row is used for sex categories.<br><br>**NOTE**: This might be useful for making data more human readable but it can easily become problematic for analysis purposes especially when using the data in applications that expect a single line header. | Convert the headers into a single line |

Examples of content problems include:

| **Type of problem** | **Problem**                                                 | **Suggested solution**                                                      |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------------|
| Content problem     | Extra white spaces in the cell value                        | Trim/remove the extra white spaces.                                         |
| Content problem     | Wrong or inconsistent use of case (lower, UPPER, CamelCase) | Convert the text to the case of choice (lowercase, UPPERCASE, Proper Case). |
| Content problem     | Spelling mistakes                                           | Correct the spelling. You can use a spell checker.                          |
| Content problem     | Missing, incorrect, or blank values                         | Find, verify, and add the correct values.                                   |

```yaml remark
type: success
text: You can always refer to <a href="https://github.com/Quartz/bad-data-guide"><strong>The Quartz guide to bad data</strong></a> for an exhaustive reference to problems seen in real-world data along with suggestions on how to resolve them.
```

```yaml remark
type: primary
text: What other formatting or content problems have you encountered when working with data?
```

### Tools and techniques
- **Spreadsheet applications** - LibreOffice Calc, Google Sheets, Microsoft Excel 
- **Specialized tools** - [OpenRefine](https://openrefine.org/)
- **Programming** - Python, R, etc

```yaml remark
type: success
text: <strong>Which tool should I use?</strong><br>Stick with <strong>what you’re comfortable with</strong> and try to <strong>start with the simplest tool first</strong> You don't need to dive directly to using specialized tools or programming. For most data work, using a spreadsheet application will be more than enough.
```

```yaml remark
type: success
text: <strong>Best practices when cleaning data</strong><ul><li>Always back-up your data.</li><li>Make a copy for every step of the cleaning process (e.g. a tab in a spreadsheet for each step).</li><li>Avoid deleting or overwriting data.</li><li>There is no such thing as over-documentation.</li></ul>
```

## Common issues
### Not keeping track of the history of modifications (i.e. version control)
A lot of the data work done by with data deals with small datasets, processed in spreadsheets. Although spreadsheets are convenient, they do not provide a history of the modifications applied to the dataset, leading to problems if a mistake was made in the process. An easy way to address this is to create a new tab every time an important modification is applied to the data. This technique is especially useful for data cleaning.

More tech-savvy data practitioners might use a version control system like GitHub or GitLab for the same purpose.
