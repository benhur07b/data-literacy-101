# Present
> Who is my audience, what message do I want to convey to them, and what is the best way for me to convey that message?

Presenting data is all about thinking of your audience, the questions you set out to answer in your project, and the medium you select to convey your message or start your conversation. Often the presentation will require a graph of some sort but that’s not always true.

The first question that you have to ask yourself at this stage of the data pipeline is not "how do I visualise the data?" but rather "what do I want my audience to get out of my project?". Put another way, **the key parameters of data presentation are your audience and your message**. Once you've properly identified the two, the process of selecting how you present the data should be easier—*not necessarily easy per se*—compared to if you didn't think about your audience and message. 

```yaml remark
type: success
text: The use of the term <strong>data presentation</strong> instead of data visualization in the Data Pipeline is deliberate. The goal when working with data is to effectively present and communicate what the data says—and that doesn't always require the use of a chart or graph. Similarly, as you might have noticed already, visualizations aren't exclusive to this step of the pipeline as they are also frequently used during data verification and analysis as well.
```

## Things to consider
### The goals of the project
What you want to achieve from the project will affect the way you will present data. Do you want to build a dashboard? Use it for an advocacy campaign? Help in the internal decision-making of your organization? Each of these will have different needs in terms of data presentation—an advocacy campaign using street demonstrations may require the use of big, bold statistics written on signs to achieve maximum impact instead of a carefully crafted chart or graph. 

At the same time, you may choose to present the same dataset in different ways depending on your audience:
- when using it in report, you may choose to include a table and a simple graph
- when presenting it to a specialized or expert audience, you may prefer the use of more complex or interactive visualizations
- when it's for the general public, you might want to create an infograghic

### Put the audience first
Always think about your audience when planning or creating your data presentation. If you can, consult and communicate with them at each step of your creative process. Show them your drafts, ask them for comments or suggestions to improve your messaging, do user-testing with a subset of your expected audience. At the end of the day, **the success of your data presentation is not up to you but to your audience**.

### Iterate to refine your visualization
**Don't rush to publish a visualization** especially one that deals with complex and nuanced issues. Unless you are a data visualization expert with decades of experience, you will make mistakes or overlook some things on the first data visualization you create for a project. Don't be scared to iterate. This may take more time but it also means that the final data presentation you publish will be more robust and fit-for-purpose.

### Choosing your visualization
**Different visualizations have different strengths and weaknesses**—some work best with categorical data while others specialize in showing trends in the data. The visualization you choose will depend a lot on the data you have and the relationships in your data. This is why it is imperative that you know how to choose the visualization or chart that will best deliver your message. Oftentimes, this means going beyond the default visualization options offered to you by spreadsheet applications. 

**But how do you choose your visualization?** One of the best teachers is experience—the longer and deeper you are involved in the world of data visualization, the easier it is for you to choose what works best for a specific scenario. But what if you're a beginner? Well, reading and research goes a long way if you have the time for it. Studying and compiling other successful data visualizations, especially those with similar context and topics to your project, is useful when you are trying to look for inspiration (think mood board). Lastly, if you are pressed for time, you can always consult data visualization catalogs for advise on what visualization to use for each kind of data and relationship you want to show. Most of these are data visualization catalogs are available online and some even give you the step-by-step guide on how to create the visualizations in different applications.

### Tools and techniques
The tools and techniques you will use will depend on the presentation or visualization you want to create. Some of these are:

**Spreadsheet applications**
- [LibreOffice Calc](https://www.libreoffice.org/)
- [ONLYOFFICE Spreadsheet](https://www.onlyoffice.com/)
- [Google Sheets](http://sheets.google.com)
- Microsoft Excel

**GIS and mapping applications**
- [QGIS](https://qgis.org/)
- [Leaflet](https://leafletjs.com/)
- [MapLibre](https://maplibre.org)
- [Mapbox](https://www.mapbox.com/)

**Web-based visualization and design applications**
- [Datawrapper](https://www.datawrapper.de/)
- [RAWGraphs](https://www.rawgraphs.io/)
- [Canva](https://www.canva.com/)
- [Google Data Studio](https://datastudio.google.com)

**Progamming**
- Python
- R

**Design and image processing applications**
- [GIMP](https://www.gimp.org/)
- [Inkscape](https://inkscape.org/)
- [Krita](https://krita.org/en/)
- Abobe Creative Cloud products

**Data visualizaton catalogs**
- [The Data Visualisation Catalogue](https://datavizcatalogue.com/)
- [From Data to Viz](https://www.data-to-viz.com/)
- [Data Viz Project](https://datavizproject.com/)
- [Chartmaker Directory](https://chartmaker.visualisingdata.com/)
- [Python Graph Gallery](https://python-graph-gallery.com/)
- [R Graph Gallery](https://www.r-graph-gallery.com/)

```yaml remark
type: success
text: You can refer to the <strong><a href="../better-data-presentations/introduction.html">Making Better Data Presentations</a></strong> part of this website for tips on how to <strong>improve your data visualizations</strong>.
```

```yaml remark
type: success
text: You can refer to the <strong><a href="../free-and-open-source-tools/introduction.html">Free and Open Source Tools</a></strong> part of this website for more information about <strong>free and open source software and applications that you can use in your data-driven project</strong>.
```

## Common issues
### Failure to identify and segment the audience of the presentation
A visualisation is not meant to be a neutral presentation but one that is able to spark discourse, conversation, and ideas in your audience. Communicating different aspects of your results to different audiences will, most of the time, require you to utilize different visualization techniques—a chart that works for one group of people may not work for another. When preparing a data visualization, you must consider not only the data and the elements you want to emphasize but als the context of the presentation and the data visualization literacy of your audience. A [sunburst chart](https://datavizcatalogue.com/methods/sunburst_diagram.html) looks very nice on screen, but is useless for an audience seeing for 30 seconds on a slide from 2 meters of distance.

### Overuse of standard chart types
It is very common for a project—especially one without a dedicated data visualization member on the team—to simply use the default chart chosen by their spreadsheet application (e.g. Excel, Google Sheets) to visualize their data. Although a bar chart, line gragh, and pie chart can be read and understood by most people, that does not mean that they are always the best options to convey a message. A very common mistake is using a pie chart with too many categories that some slices end up so small and there is no way to make sense of them visually thus defeating the purpose of using a data visualisation.

Read more: https://eagereyes.org/techniques/pie-charts 

### Common dataviz mistakes
Choosing a chart that does not emphasize the right message is a strategic mistake, but some errors can be more problematic, as they lead your data visualisations to become misleading.

```yaml remark
type: success
text: You can refer to the <strong><a href="../better-data-presentations/introduction.html">Making Better Data Presentations</a></strong> part of this website for tips on how to <strong>avoid common data visualization mistakes</strong>.
```
