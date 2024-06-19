---

layout: page
title: Graph Summarizer
description: A project focused on generating concise summaries of complex graphs to enhance data understanding and decision-making.
img: assets/img/bargraph.png
category: Python

---


### Overview
The Graph Summarizer project aims to simplify complex graph data into concise summaries, making it easier to visualize, understand, and make data-driven decisions.

### About the Project
The tool is designed to take images of graphs, extract key information, and generate a PDF summary. This project currently supports bar graphs and line graphs, with plans to include other types of graphs in the future.

### How It Works
1. **Input**: Provide the path to the graph image.
2. **Processing**: The tool extracts data from the graph and analyzes it.
3. **Output**: A summary is generated and saved as a PDF.

### Usage
Run the following command to summarize a bar graph:

```sh
python plot.py summarize bargraph.png bargraph
```

For a line graph:

```sh
python plot.py summarize linegraph.png linegraph
```
### GitHub Repository

Explore the source code and contribute to the project on GitHub:
<a href="https://github.com/ughrima/Graph_summarizer" class="btn btn-secondary" target="_blank">View on GitHub</a>


### Sample Outputs

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/bargraph.png" title="Bar Graph Sample" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/linegraph.png" title="Line Graph Sample" class="img-fluid rounded z-depth-1" %}
    </div>

</div>
<div class="caption">
    Above are the sample graphs, and below is the sample PDF generated for the bar graph.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sample-pdf.png" title="PDF Summary Sample" class="img-fluid rounded z-depth-1" %}
    </div>
        </div>


### Future Scope
- Support for additional graph types (e.g., scatter plots, area graphs).
- Extension to 3D and 4D graph summaries.


### Tech Stack
- **Python**

---