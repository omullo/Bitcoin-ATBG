
# README for Bitcoin-ATBG Visualization Notebook

## Overview

This Jupyter Notebook is designed to visualize a bipartite graph representing Bitcoin transactions and addresses using the `ipycytoscape` library. The dataset contains transactions from January 3, 2009, to June 7, 2018. It maps addresses and transactions from the raw Bitcoin blockchain to numerical vertex IDs, creating a comprehensive bipartite graph.

## Dataset Information

**Name**: Bitcoin-ATBG

**Description**: The dataset is a Bitcoin address-transaction bipartite graph, spanning over 9.5 years of transactions. It includes mappings from Bitcoin transactions and addresses to numerical vertex IDs. This bipartite graph consists of:
- **Transactions**: 321,043,952 (321 million)
- **Addresses**: 399,344,696 (399 million)
- **Total Vertices**: 720,388,650 (720 million)
- **Total Edges**: 1,692,308,191 (1.6 billion)

**Formats**:
1. **Matrix Market Exchange Format (.mtx)**: ASCII file format.
2. **Compressed Sparse Row (CSR)**: Binary format.
3. **Sample Graphs**: Included in both Matrix Market and CSR formats for demonstration.

## Notebook Instructions

### Purpose

The notebook demonstrates the following:
1. Fetching and parsing JSON data from an API.
2. Processing and extracting relevant parts of the dataset.
3. Creating node and edge data structures.
4. Visualizing the bipartite graph using `ipycytoscape`.

### Setup and Running the Notebook

1. **Install Jupyter Notebook**:
   Ensure you have Jupyter Notebook installed. If not, install it using pip:
   \`\`\`sh
   pip install notebook
   \`\`\`

2. **Install Required Packages**:
   Install the necessary Python packages:
   \`\`\`sh
   pip install requests pandas ipycytoscape
   \`\`\`

3. **Launch Jupyter Notebook**:
   Start Jupyter Notebook from the command line:
   \`\`\`sh
   jupyter notebook
   \`\`\`

4. **Open and Run the Notebook**:
   - Open the provided notebook file in Jupyter Notebook.
   - Execute each cell sequentially to fetch data, process it, and visualize the graph.
   - The final cell will display the bipartite graph using `ipycytoscape`.

## Conclusion

This notebook provides a comprehensive guide to processing and visualizing a subset of the Bitcoin-ATBG dataset. It showcases the use of `ipycytoscape` to handle and visualize large bipartite graphs within a Jupyter Notebook environment.
