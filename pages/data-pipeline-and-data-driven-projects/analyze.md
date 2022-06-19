# Analyze
> What do I want to get from my data?

Here we are! Data analysis is generally what comes to mind when we think about "working with data" but as you might have noticed, the actual analysis only comes at the end of a multi-step process. You will also find that **if you were able to do the previous steps of the pipeline correctly, the data analysis step becomes easy and trivial**. That is not to say that analysing data is always easy. Depending on the goals of your project and the data you have, it can also become something that only seasoned statisticians can undertake. 

Luckily, most of the analysis questions that you will encounter can be tackled with simple tools. If your questions look like ‘who is most affected by X?’ or ‘how has Y evolved over the years?’ then you will most likely be able to answer them yourself. If instead your question is of the ‘is X influenced by Y’ kind, then you will most likely need the help of someone with statistics training to help.

```yaml remark
type: success
text: <strong>You can think of the analysis step as you interviewing the data</strong> and the previous steps of the pipeline as preparation for the interview. Instead of a microphone, you will use a spreadsheet. Instead of questions, you have spreadsheet formulas. 
```

## Things to consider
### The type of analysis you need
There are three general types of data analysis:

**1. Descriptive analysis** that focuses on describing the basic features or characteristics of the data, such as the mean, the median, the maximum, the minimum, etc.

**2. Inferential analysis** which allows you to make reasonable guesses about your data and how it relates to the larger dataset that it is part of or other datasets that are similar to itself.

**3. Predictive analysis** is an advanced type of analysis where the goal is to make reasonable predictions about the probability of future or otherwise unknown events based on current or past data.

### Tools and techniques
The kinds of tools and techniques you will use depends on your goals and data. If you are working mostly with tabular data in order to perform descriptive analysis, a spreadsheet application would suffice. The more complex or specialized your goals and data are, the more complex and specialized tools and techniques you would require. Some of these include:
- **Programming languages** such as Python and R if you need complex, advanced, and automated computations.
- **Databases and SQL** if you are dealing with large amounts of data and you need a scalable and robust storage + analysis solution.
- **GIS and geospatial applications** if you are dealing with geospatial/location data, location is an important variable in your analysis, or you just want to make maps
- **Statistical software** such as SPSS and Stata for more advanced statistical analysis.

```yaml remark
type: success
text: For a complex data project, a single tool may not be enough and you would need to use different kinds of tools and techniques to analyze your data. It's okay to seek help with tools that you may not be familiar with or are not comfortable using.
```

### Using a hypothesis
There are many ways to twist and turn the data to get some sort of answer but this should be discouraged or you run the risk of doing [data dredging](../common-issues/data-fallacies.html) instead of data analysis. Having a well-defined research question helps guide your analysis of the data and having hypotheses when doing your analysis helps you make sense of and interpret the results. 

Using a hypothesis makes you more deliberate with your analysis and prevents you from becoming arbitrary in your approach. Your hypothesis will tell you what to test/compute and how to interpret the results in the context of your project. It will tell you if the assumtions you made about your data or your project are valid. Additionally, even if the results of your analysis tells you to reject the hypothesis you made, this outcome is still interesting and significant because it means that the data does not say what you expected it to. 

The hypotheses you set can be based on previous analyses or expectations of what the data should show. 

### Documenting the analysis
Many teams rush to the analysis part and end up producing results that are hardly verifiable or reproducible because of the chaotic process they used to analyse the data. Documenting that process forces the analyst to organise their steps, and, sometimes, helps catch mistakes in the process.

### Making the analysis reproducible
There are several ways for you to ensure that your project is reproducible such as following the [FAIR](../open-data/beyond-open-data.html#fair-findable,-accessible,-interoperable,-reusable-principles) principles or using technologies such as [Frictionless](../open-data/beyond-open-data.html#frictionless-data).

Take note however that this isn't just limited to the analysis step of the data pipeline as reproducibility should be considered at all phases of your data-driven project—e.g. planning for your project to be reproducible from the start.

## Common issues
## Not using hypotheses
While a research question helps refine the direction and scope of a project, hypotheses help guide the data analysis. An insight generated from a data analysis can only make sense when replaced in the context of the topic being studied. What does it mean if, when studying public procurement, you find that 50% of contracts are won by only 10% of the total number of suppliers who submitted bids? Is it a lot or too little? Good or bad? Making a hypothesis (e.g. there is healthy competition when at least 25% of the suppliers win 50% of the contracts), based on past data or prevailing assumptions about the topic, helps frame the results of the analysis. Whether the hypothesis is verified or not, the results can now make sense.

## No documentation of the analysis steps
You can never have too much documentation. This does not need to be overly verbose or complicated but should be complete and understandable enough to allow for the verification and review of the analysis steps or the reuse, replication, and reproduction of the steps in another project.