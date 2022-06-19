# What is data?
> “Data may be thought of as **unprocessed atomic statements of fact**.” ([Open Data Handbook](https://opendatahandbook.org/glossary/en/terms/data/))

The definition above is just one of the many definitions that you will find if you search for the meaning of data. We all have an instinctive sense of what data is but if you ask different people to define it, you will get different answers. That much is sure. Now even though not having a singular definition does not prevent us from properly using data, when we are just starting to learn about data, it is important that we have a clear definition that we can agree on. 

For this module, aside from the definition from the Open Data Handbook, we will also define data as **structured representations of the world**.

## A structured representation of the world
```yaml remark
type: success
text: In this website, a <b>data point</b> refers to individual elements collected about reality (i.e. age being one data point about a a person) while a <b>dataset</b> refers to a collection of data points (i.e. a dataset can include a person's age, name, address, etc.).
```

Data is **structured** because it follows logical and well-defined rules as to how it is stored or presented. It is this structure that differentiates data from other pieces of information such as a textual description. For example, the statement "Jose is a 35-year-old male living in Pampanga." can be restructured into a table with fields for ```name``` (Jose), ```age``` (35), ``sex`` (male), and ``location`` (Pampanga).

Data is a **representation of the world** because it tries to capture a part of reality. It is important to remember that no matter how large of a dataset you gather, it is always almost impossible to represent reality in its entirety. This is why it is important in any data project to always [verify](../data-pipeline/verify.html) if the data that will be used and the outcomes from analyzing the data are valid and appropriate. There are several ways to do this which include getting expert advice, consulting the source of the data, and performing preliminary statistical analysis.

**Non-structured representation**

Jose is a 35-year-old single male living in Pampanga while Maria is a 29-year-old married female living in Antique.

**Structured representation**

```yaml table
data:   [{"name": "Jose", "age": 35, "civil status": "single", "sex": "male", "location": "Pampanga"}, 
        {"name": "Maria", "age": 29, "civil status": "married", "sex": "female", "location": "Antique"}]
width: 720
columns:
  - data: name
  - data: age
  - data: "civil status"
  - data: sex
  - data: location
```
<br>

```yaml remark
type: warning
text: Structured and unstructured data may have different definitions in other fields such as data science.
```

```yaml remark
type: warning
text: It is not always true that structured = quantitative and non-structured = qualitative. For example, you can have a structured dataset of qualitative information.
```

## Classifications of data
There are several ways to classify data and the more you work with data, the more you will be familiar with these classifications. One of the most common ways that data is classified is whether it provides **quantitative** or **qualitative** information.

Data as a term is used in multiple ways in multiple disciplines. In casual conversations, data is often used interchangeably with information while in a more technical or scientific setting, data pertains to information collected in a structured way. Specifically:

**Qualitative data** is data that refers to the quality of something: the name of a person, the name of a company, a description of experiences are all qualitative data. It can be unstructured (e.g. interview transcription) or structured (e.g. a table organizing information from the interview).

**Quantitative data** is data that refers to a number—e.g. the age of a person, the number of bidders for a project, the amount of the winning bid are all quantitative data.

Data can also be classified based on the **type of information** it holds. For example:

**Numerical data** uses numbers to hold information. They can further be classified into:
- **Discrete data** which is numerical data with distinct values or gaps between them. These usually come in the form of counting numbers or integers. Examples include the number of bidders for a government project, the age of a person in years, or the number of correct answers in an exam.
- **Continuous data** which is numerical data with a continuous range. These usually take the form of rational numbers. Examples include the height of a person, the length of your foot in cm or inches as opposed to your shoe size which is discete, or the amount of the winning bid for a government project.

**Categorical data** puts the object being described into a category. In the case of Jose and Maria, their civil status and sex are categorical data about them.

Other types of data that you may encounter are: **Geographic or Spatial data** that hold information connected to a particular place or location and **Time-series data** which holds information about the value/state of a particular thing over time.

```yaml remark
type: primary
text: Think of a common dataset that you use at work (or common information that you gather), how do you classify these information? Are they numerical, categorical, spatial, or maybe some other kind of data?
```

## The value of data
<figure>
<img src="https://www.theifactory.com/wp-content/uploads/2019/01/Data-Wisdom-768x250.jpg">
<figcaption><i>Gaining wisdom from data by the <a href="https://www.theifactory.com">Information Factory</i></a></figcaption>
</figure>

You have probably encountered the diagram above from the [Information Factory](https://www.theifactory.com/news/gaining-wisdom-from-data/) before. It illustrates that it is not the data per se that has value but it is what you do with the data that counts.

- **Data** starts as seemingly random dots that could represent anything.
- **Information** is generated when meaning and attributes are attached to the raw data indicated by applying different colors to the dots.
- **Knowledge** is gained when the dots start to make sense and connections between the different pieces of information can be made.
- **Insight** is when knowledge become synthesized in order to obtain a deeper understanding of the data or the problem—i.e. identifying the two most important dots in the set.
- **Wisdom** is then the ability to use insight in order to facilitate informed decision making—i.e. finding the best path between two dots.

**Data is valuable** not because it is data but **because of the things that we can gain from it**.

```yaml remark
type: primary
text: <b>Let's play a game:</b><br>I have a box in front of me.<br>The box is large and heavy.<br>There’s a door in front of the box which I can open.<br>A light comes on when I open the door.<br>The inside of the box is colder than the outside.<br>There is usually food inside the box.<br>The box is usually found in the kitchen.<br>There are usually things put on top of the box.<br><br><b>What is the box?</b>
```

At some point in the game above, you managed to connect the different pieces of information (knowledge) to formulate a hypothesis (insight) about the box. By combining these pieces of information together, you are able to arrive at an informed decision about what the box is. If you guessed refrigerator, then you are right. 

However, did you ever think about the fact that this answer—that the box is a refrigerator—only makes sense because we live in a society that knows what a refrigerator is and its characteristics? If you show the same set of statements to people who have never seen or heard of a refrigerator, would they give you the same answer? This brings us to our next point about the value of data: **data is only valuable when put in the proper context**. This means that the data you use to solve one problem may not be useful for solving a different problem or even the same problem in a different context. This is why it is imperative in any data-driven project that we properly [define the problem we are trying to solve](../data-pipeline/define.html) before proceeding with gathering, analyzing, or visualizing the data.

Data also becomes **valuable when you can turn data into action**. Here it is important to note that we cannot act on what we cannot measure. This is why [finding](../data-pipeline/find.html) and [getting](../data-pipeline/get.html) the appropriate data is important if we plan to make data actionable.

## The (ab)use of data

- Data is a resource (such as energy, oil, people) and like any resource, data is susceptible to both use and abuse.
- Data can and will lie. See: [Data fallacies](../common-issues/data-fallacies.html)
- [Data ethics](../data-ethics/introduction.html) should be an integral consideration in any data activity especially those that have the potential to affect people and communities directly or indirectly. The way that data is collected, shared, and used should consider issues such as openness, consent, bias, and privacy.

## The field of data is far too important to be left to data scientists

Because of the ubiquity, value, usefulness, and susceptibility for abuse of data, it is imperative that everyone is involved in the conversations around data. In order to fulfill the promise and potential that data has to offer, a data literate citizenry is needed where everyone—civil society organizations, businesses, local governments, journalists, citizens—understands what data is and uses it effectively to perform their civic duties and participate in society. This is where [data literacy](../data-literacy/introduction.html) comes in.

The field of data should be inclusive and no single person, department, or organization should have a monopoly on data because **the field of data is far too important to be left only to data scientists**.

> "<b>Data are like the stars.</b> They are all around us even when we don’t see them; when we do see them, they might seem incomprehensible but if we look hard enough, we can connect them to see patterns and constellations." (adapted from the answer of a participant from one of my Data Literacy training-workshops in South Cotabato when asked to explain the concept of data to a five-year old)

```yaml remark
type: primary
text: How about you? What is your own definition of data?
```