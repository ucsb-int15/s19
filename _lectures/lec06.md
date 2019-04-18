---
num: "lect06"
lecture_date: 2019-04-18
desc: "Data Visualization"
ready: true
reading: "Fundamentals of Data Visualization"
pdfurl: 
---

## Lecture References
The newly released book: [Fundamentals of Data Visualization](https://serialmentor.com/dataviz)
Lecture featured examples from Chapters 2-5 and 29.

The article from _The Economist_ about their visualisations: [Mistakes, we’ve drawn a few](https://medium.economist.com/mistakes-weve-drawn-a-few-8cdd8a42d368)a

## Anscombe's Quartet
[Anscombe's Quartet](https://en.wikipedia.org/wiki/Anscombe%27s_quartet), developed by F.J. Anscombe in 1973, is a set of four datasets that have nearly the same summary statistics (mean, standard deviation, and correlation) but, when plotted, result in very different graphs.

Add the following code to a new notebook in JupyterHub and verify it for yourself (compute the summary statistics too):
```python
"""
Anscombe's quartet
==================
"""
import seaborn as sns
sns.set(style="ticks")

# Load the example dataset for Anscbombe's quartet
df = sns.load_dataset("anscombe")
df

#######
# Show the results of a linear regression within each dataset
sns.lmplot(x="x", y="y", col="dataset", hue="dataset", data=df,
           col_wrap=2, ci=None, palette="muted", height=3,
           scatter_kws={"s": 50, "alpha": 1})
```

Alberto Cairo created the Datasaurus dataset "to illustrate how important it is to visualize data while analyzing it":
[Download the Datasaurus: Never trust summary statistics alone; always visualize your data](http://www.thefunctionalart.com/2016/08/download-datasaurus-never-trust-summary.html)

Interesting results from Autodesk Research: [Same Stats, Different Graphs: Generating Datasets with Varied Appearance and Identical Statistics through Simulated Annealing](https://www.autodeskresearch.com/publications/samestats)
