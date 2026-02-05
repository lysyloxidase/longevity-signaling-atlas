# Longevity Signaling Atlas (WikiPathways + OmniPath)

This project builds an **interactive atlas (network map)** of cellular signaling pathways and cascades related to **longevity / healthspan**.  
The Python notebook (Google Colab) automatically pulls pathway and interaction data from public resources, constructs a molecular interaction graph, and generates interactive **2D and 3D** visualizations.

## What the notebook does
- searches and downloads “aging / longevity / healthspan” pathways from **WikiPathways**
- parses pathways (molecules + connections) and builds a network graph
- fetches directed/signed signaling interactions from **OmniPath** (optional enrichment)
- generates:
  - **interactive 2D network** (PyVis, exported as HTML)
  - **interactive 3D network** (Plotly)

## How to run (simplest)
### Google Colab
1. Open the `.ipynb` file in Google Colab
2. Run cells from top to bottom (Runtime → Run all)
3. Interactive visualizations will appear once data are loaded and the graph is built

### Local (optional)
1. Install Python 3.10+  
2. Install dependencies:
```bash
pip install pandas numpy networkx tqdm requests lxml pyvis plotly ipywidgets
