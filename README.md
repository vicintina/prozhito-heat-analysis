# "Everyone's soul is burning:" Metaphorical and Somatic Expressions of Heat in Russian-language Diaries

A Digital Humanities project tracking the semantic evolution of affective heat, fever, and somatic stress responses in Russian personal narratives (18th–21st centuries). 

This repository contains the Python NLP pipeline and visualization code used to extract, classify, and analyze somatic and metaphorical heat expressions within the [Prozhito](https://prozhito.org/) historical diary corpus. This research was prepared for the ["Feel the Heat. Science and Histories of Fever"](https://www.marsilius-kolleg.uni-heidelberg.de/de/studium/internationale-marsilius-akademien/feel-the-heat-science-and-histories-of-fever) International Marsilius Academy (Heidelberg University, 2026).

## Methodology

* **Data Extraction:** A custom NLP pipeline utilizing `PyMorphy2` and complex regular expressions to isolate records connected to the feeling of heat, while filtering out literal descriptions of weather or physical illness.
* **Taxonomy & Annotation:** A concentrated dataset of relevant records manually annotated across a three-tier taxonomy:
  * **Linguistic Form:** Poetic metaphor, somatic reaction, idiom.
  * **Emotional State:** Love, anxiety, excitement, anger, shame.
  * **Context:** Politics, religion, creation, interpersonal.
* **Temporal Tracking:** Analysis relies on relative frequencies rather than absolute counts to account for the pronounced chronological asymmetry inherent to the foundational Prozhito database.

## Visualizations Generated

The code produces several presentation-ready visualizations:
* **Data Distribution Bar Charts:** Visualizing the absolute total of selected vs. highly relevant records per historical era.
* **Context Evolution Line Chart:** Tracing the relative frequency of semantic contexts over time (highlighting shifts like the surge of political heat metaphors during the 1939–1947 wartime era).
* **Dominant Affective Pairs Heatmap:** Tracking the top form and feeling combinations across the five historical periods to visualize semantic evolution.

## Repository Structure

* `prozhito_heat.ipynb`: The main Jupyter Notebook containing the data processing, NLP pipeline, statistical calculations, and visualization rendering.
* `manual_tags.json`: The JSON file containing the manual taxonomy annotations for the extracted records.
* `Feel_the_Heat_Poster.pdf`: The final research poster presenting the methodology, insights, and visualizations, prepared for the Marsilius Academy.
* *Note:* Due to file size restrictions, the raw XML Prozhito database dump (`prozhito-dump-1`) is not hosted in this repository.

## Requirements

To run the notebook, ensure you have Python installed along with the following libraries:
* `pandas`
* `numpy`
* `nltk`
* `pymorphy2`
* `stop_words`
* `matplotlib`
* `seaborn`
* `prozhitotools`

## License

This project is licensed under the [MIT License](LICENSE). 
Written and visual content (posters, generated graphs, qualitative analysis) is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) License.
