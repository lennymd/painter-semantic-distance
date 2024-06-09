# Day 4 - Visualizing painter biographies

## 4.0 - Getting Started

### Introduction

The fourth day of this class will show you:

- [HuggingFace](https://huggingface.co/), a platform for finding and working with different machine learning models.
- How to use **DistilBERT** to visualize how similar painters are based on their short bios.

Please download the code and data from the [github repository](https://github.com/aica-wavelab/aica-assignments) and follow the instructions in the `A4_painter_semantic_distance`.

[Github repository of the course](https://github.com/aica-wavelab/aica-assignments)

### Content of the repository

- `data`: A folder containing the summary information for artists gathered from Wikipedia.
- `A4_painter_semantic_distance.ipynb`: This notebook where we will do the analysis and visualization work.

### Assignment

Today's task is to find a way to cluster and visualize painters based on the summaries\*(more on this below) of their Wikipedia pages.

@@REVIEW@@

### Installation required

Make sure you have the following packages installed for today.

- @@REVIEW@@
- pandas

---

## 4.1 - The dataset

The dataset is something I put together using the `wikipedia-api` package (linked [here](https://pypi.org/project/Wikipedia-API/)). It's a collection of the summaries from painter pages on Wikipedia. The painter pages come Wikipedia's [List of painters by name](https://en.wikipedia.org/wiki/List_of_painters_by_name). While it has a lot of painters, it's important to note that it does not cover _all_ the painters who have pages on Wikipedia.

The dataset is divided into two sections:

- The main file is `painter_summaries_all.csv`; it has data on all 3900+ painters listed in the Wikipedia article. One listed painter has been removed from this dataset that appears in the partial files and the IDs not been changed.
- There are also 6 files in the `partial` directory with the format `painter_summaries_part##.csv`. These files have the data split into smaller chunks based on how the data was gathered.

## Inspecting the data

Open `painter_summaries_all.csv` file in a spreadsheet program (Excel, Numbers, Sheets, etc) and take a look at the data.

<div class="alert alert-info">
<b>Instruction:</b> What are the columns in this dataset? What do they each contain?
</div>

YOUR ANSWER HERE

Let's load the dataset and look at it in
