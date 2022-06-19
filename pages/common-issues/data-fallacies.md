# Data fallacies
> "Statistics never lie, but lovers often do..." (J. Tinga, Antonio vs. Reyes, 484 SCRA 353 (2006))

With all due respect to Justice Tinga but **statistics and data do lie** and they do it quite often.

## Cherry picking
<figure>
<a title="Physikinger, CC0, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Global_warming_hiatus.gif">
<img src="https://upload.wikimedia.org/wikipedia/commons/f/f4/Global_warming_hiatus.gif"></a>
<figcaption><i>By selecting or cherry-picking data, the trend of global warming appears to mistakenly stop, as in the period from 1998 to 2012, which is actually a random contrary fluctuation.</i></a></figcaption>
</figure>

### What it is
- [Cherry picking](https://en.wikipedia.org/wiki/Cherry_picking) is also known as suppressing evidence or the fallacy of incomplete evidence.
- Selecting, using, and presenting only the subset of the data that agree or fit with your claims and beliefs. 
- This becomes really dangerous when paired with people’s confirmation bias.

### How to avoid it
- As a creator, always be faithful to your data and results especially when they do not fully agree with your claims.
- As a consumer, ask for the complete dataset or ask yourself: “What am I not being told?”


## Data dredging
<figure>
<a title="Tyler Vigen, CC BY 4.0 &lt;https://creativecommons.org/licenses/by/4.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Spurious_correlations_-_spelling_bee_spiders.svg"><img src="https://upload.wikimedia.org/wikipedia/commons/0/0c/Spurious_correlations_-_spelling_bee_spiders.svg"></a>
<figcaption><i>An example of data produced by data dredging through a bot operated by Tyler Vigen, apparently showing a close link between the best word in a spelling bee competition and the number of people in the US killed by venomous spiders. It's obviously a coincidence: with so many possible comparisons of data of things happening in the world, it is easy to find some unrelated data that shows similar trends.</i></a></figcaption>
</figure>

### What it is
- [Data dredging](https://en.wikipedia.org/wiki/Data_dredging) refers to the misuse of data analysis to find patterns in data that can be presented as statistically significant.
- Seeking correlation where there is none. Performing countless statistical tests on data and reporting the ones that show correlation.
- If you combine enough time with a large enough dataset, you are bound to find things that appear to be correlated.

### How to avoid it
- Always be upfront with what you are testing—e.g. using a hypothesis in the analyze step of the data pipeline.
- Accept that sometimes things that seem to be correlated aren’t.

## Survivorship bias
<figure>
<a title="Martin Grandjean (vector), McGeddon (picture), Cameron Moll (concept), CC BY-SA 4.0 &lt;https://creativecommons.org/licenses/by-sa/4.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Survivorship-bias.svg"><img src="https://upload.wikimedia.org/wikipedia/commons/b/b2/Survivorship-bias.svg" width="900px"></a>
<figcaption><i>This hypothetical pattern of damage of returning aircraft shows locations where they can sustain damage and still return home. If the aircraft was reinforced in the most commonly hit areas, this would be a result of survivorship bias because crucial data from fatally damaged planes was being ignored; those hit in other places presumably did not survive.</i></a></figcaption>
</figure>

### What it is
- [Survivorship bias](https://en.wikipedia.org/wiki/Survivorship_bias) is the logical error of drawing conclusions from an incomplete dataset composed of data that has survived a selection process and overlooking those that did not, typically because of their lack of visibility.
- Example:
    - Bullet patterns of WW2 aircrafts returning from the war
    - College dropouts being billionaires—for every 1 dropout who ended up becoming a billionaire, how many thousands more did not?

### How to avoid it
- Always try to look at the full picture and ask yourself if you are overlooking anything or if something is missing in your data.
- Ask yourself: "Did your data undergo any selection or trimming process prior to your analysis?"

## Sampling bias
<figure>
<a title="Sampling Bias, via Geckoboard" href="https://www.geckoboard.com/best-practice/statistical-fallacies/"><img src="https://www.geckoboard.com/assets/img/data_fallacies/sampling-bias-data-fallacy-illustration-geckoboard.png" width="720px"></a>
<figcaption><i>Sampling Bias, via <a href="https://www.geckoboard.com/best-practice/statistical-fallacies/">Geckoboard</a></i></a></figcaption>
</figure>

### What it is
- [Sampling bias](https://en.wikipedia.org/wiki/Sampling_bias) occurs when a sample is selected in a way such that some members of the intended population have a lower or higher chance of being included in the sample.
- Results in conclusions drawn from a dataset that is not representative of the population you are trying to understand.
- Example:
    - Using an online poll to determine whether students are in favor of online classes.

### How to avoid it
- Always try to use a representative sample of your population in your analysis. 
- Choose an appropriate and robust sampling method.

## Cobra effect
<figure>
<a title="The cobra effect, via sketchplanations" href="https://sketchplanations.com/the-cobra-effect"><img src="https://images.prismic.io/sketchplanations/3b872f06-7ade-4713-bf9e-487e5605f5d0_186110724996.jpg?auto=format&ixlib=react-9.0.3&h=1887.557603686636&w=1600&q=75&dpr=1" width="600px"></a>
<figcaption><i>The story goes something like this: back in colonial India the top Brit in charge decided there were too many cobras around Delhi. To reduce the population they put in place a cash reward, or bounty, for anyone who brought in a dead cobra. The intention was clear. Legend has it that people did bring in the cobras reliably because some enterprising souls had started breeding cobras for the very purpose of getting the bounty.</i></a></figcaption>
</figure>

### What it is
- When an attempted solution to a problem somehow makes it worse as an unintended result of using incorrect stimulation or wrong incentives.
- [Other examples](https://en.wikipedia.org/wiki/Perverse_incentive#The_original_cobra_effect).

### How to avoid it
- Be careful what you are incentivizing because incentives generally increase the likelihood of what you are incentivizing.

## Gerrymandering / MAUP
<figure>
<a title="M.boli, CC BY-SA 4.0 &lt;https://creativecommons.org/licenses/by-sa/4.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:DifferingApportionment.svg"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/DifferingApportionment.svg/406px-DifferingApportionment.svg.png"></a>
<figcaption><i>Different ways to apportion electoral districts leads to different election results</i></a></figcaption>
</figure>

### What it is
- In both [gerrymandering and the Modifiable Areal Unit Problem (MAUP)](https://en.wikipedia.org/wiki/Gerrymandering), the outcome of an event (e.g. election, analysis) can vary depending on how you divide the area of interest.

### How to avoid it
- Always consider the scale and how you group your data when doing your analysis. Try to see if your results also vary when you vary your scale.

## False causality
<figure>
<a title="False Causality, via Geckoboard" href="https://www.geckoboard.com/best-practice/statistical-fallacies/"><img src="https://www.geckoboard.com/assets/img/data_fallacies/false-causality-data-fallacy-illustration-geckoboard.png" width="720px"></a>
<figcaption><i>False Causality, via <a href="https://www.geckoboard.com/best-practice/statistical-fallacies/">Geckoboard</a></i></a></figcaption>
</figure>

### What it is
- The belief that because two events occur together or immediately after one another then one must have caused the other.
- Correlation does not imply causation. 

### How to avoid it
- Never assume causation based on correlation alone.

## Danger of summary metrics
<figure>
<a title="Anscombe's quartet, via Wikimedia user Schutz" href="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Anscombe%27s_quartet_3.svg/1024px-Anscombe%27s_quartet_3.svg.png"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Anscombe%27s_quartet_3.svg/1024px-Anscombe%27s_quartet_3.svg.png" width="720px"></a>
<figcaption><i>Four different datasets look identical when examined using simple summary statistics, but vary considerably when graphed.</a></i></a></figcaption>
</figure>

### What it is
- Reliance on summary metrics blur out differences in the dataset. Some datasets may have the same summary metrics (e.g. mean, variance, correlation) but be totally different from each other.
- Example:
    - [Anscombe’s quartet](https://en.wikipedia.org/wiki/Anscombe%27s_quartet)

### How to avoid it
- As a provider, show or open the data used for the study instead of just the summary statistics.
- As a consumer, always look or ask for the data behind the summary statistics used.

## Other data fallacies
- [**Simpson's paradox**](https://en.wikipedia.org/wiki/Simpson%27s_paradox) - A phenomenon in probability and statistics in which a trend appears in several groups of data but disappears or reverses when the groups are combined.
- [**Gambler's fallacy**](https://rationalwiki.org/wiki/Gambler's_fallacy) - The erroneous belief that if an event occurs more frequently than normal in the past then it is less likely to occur in the future, when it has already been established that the probability of such events do not depend on what happened in the past.
- [**Hawthorne effect**](https://en.wikipedia.org/wiki/Hawthorne_effect) - Also known as the Observer Effect. This is the phenomenon where the actions and behaviors of the subjects of a study change because they are aware that they are being observed/monitored.
- [**McNamara fallacy**](https://www.logicallyfallacious.com/logicalfallacies/mcnamara_fallacy.html) - Being too focused on what can easily observed and assuming that does that cannot are irrelevant. This leads to decisions based solely on quantitative observations (i.e., metrics, hard data, statistics) while all qualitative factors are ignored.
- [**Publication bias**](https://en.wikipedia.org/wiki/Publication_bias) - Refers to the fallacy that the outcome of a research or experiment influences whether it is published instead of the robustness of the methodology. This results in an imbalance in published papers in favor of positive results when, in reality, more researches using the same methodoly but showing negative or inconclusive results may exist.


```yaml remark
type: success
text: For more information, you can refer to <strong><a href="https://www.geckoboard.com/best-practice/statistical-fallacies/">Data fallacies</a></strong> by Geckoboard.
```