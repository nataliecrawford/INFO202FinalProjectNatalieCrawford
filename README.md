# INFO 202 Final Project: Travel Scrapbook

**Natalie Crawford**

A faceted image collection of travel photos, with a hand-built facet taxonomy, a hand-labeled sample, classifier-predicted labels for the full collection, and a faceted browser for exploring it.

🔗 **Live site:** https://nataliecrawford.github.io/INFO202FinalProjectNatalieCrawford/

---

## Contents

| Component | Location | Status |
|---|---|---|
| Data (images + captions) | `data/` | ✅ |
| Hand-classified sample | `Hand_Classified_Sample.csv`, `facetlabeling/HandLabeled_NatalieCrawford.csv` | ✅ |
| Faceted browser | `facetbrowser_nataliecrawford.html` | ✅ |
| Classification code + output | `classification/` | ✅ |
| Retrieval system, query set, relevance judgments | `retrieval/` | **TODO** |
| Written report | `report/` | **TODO** |

---

## 1. Data

- **Images:** `data/images/`. The full collection, named by location (for example `amalfi_image1.JPG`, `barcelona_image1.JPG`).
- **Captions:** `data/imagecaptions.tsv`. One caption per image.
- **All labels:** `facetlabeling/AllLabels_NatalieCrawford.csv`.

## 2. Taxonomy and Hand-Classified Sample

- **Facet definitions:** [`facetlabeling/FacetDefinitions_NatalieCrawford.pdf`](facetlabeling/FacetDefinitions_NatalieCrawford.pdf)
- **Hand-labeled ground truth:** `Hand_Classified_Sample.csv` and `facetlabeling/HandLabeled_NatalieCrawford.csv`
  - **TODO:** say which file is the ground truth used by the classifier, or remove the duplicate.
- **Browsable view:** [Hand-Labeled Sample](https://nataliecrawford.github.io/INFO202FinalProjectNatalieCrawford/facetlabeling/LabelingFilesHtmls/hand_labeled.html)

## 3. Faceted Browser

- **Live version:** [Faceted Browser](https://nataliecrawford.github.io/INFO202FinalProjectNatalieCrawford/facetbrowser_nataliecrawford.html)
- **Source:** `facetbrowser_nataliecrawford.html`

**How to run it:** the browser is a single self-contained HTML file with no server, install or live service needed. Either:
1. Open the live link above, or
2. Download or clone this repo and open `facetbrowser_nataliecrawford.html` in any web browser.

The file is about 32 MB, so it may take a few seconds to load.

## 4. Classification

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nataliecrawford/INFO202FinalProjectNatalieCrawford/blob/main/classification/final_project_classifier_nataliecrawford.ipynb)

- **Notebook:** `classification/final_project_classifier_nataliecrawford.ipynb`. It's too large for GitHub to preview, so use the Colab button above or the [PDF version](classification/final_project_classifier_nataliecrawford.ipynb%20-%20Colab.pdf).
- **Predicted labels (output):**
  - `classification/predicted_labels_alldata_nataliecrawford.csv`
  - `facetlabeling/PredictedLabels_NatalieCrawford.csv`
- **Browsable views:**
  - [Classifier Predicted Labels](https://nataliecrawford.github.io/INFO202FinalProjectNatalieCrawford/facetlabeling/LabelingFilesHtmls/predicted_labels.html)
  - [Full Collection Labeled](https://nataliecrawford.github.io/INFO202FinalProjectNatalieCrawford/facetlabeling/LabelingFilesHtmls/full_info.html)

**How to run it:** open the notebook in Colab and run all cells.
- **TODO:** list any input files the notebook expects and where to put them (for example, upload `Hand_Classified_Sample.csv` and `data/imagecaptions.tsv` to the Colab session).
- **TODO:** briefly describe the method (model or features used) and how its output compares to the hand-built facets.

## 5. Retrieval System — TODO

- **TODO:** retrieval system code
- **TODO:** query set
- **TODO:** relevance judgments file
- **TODO:** how to run it

## 6. Written Report — TODO

- **TODO:** upload the report (about 2000 words, excluding citations), covering:
  - the taxonomy and its theoretical grounding
  - the faceted browser
  - the classification experiment compared against the hand-built facets
  - the retrieval system and its evaluation
  - a reflection on what the scheme silences
