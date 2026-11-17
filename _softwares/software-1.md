---
layout: software
title: "ZSS: Zotero Similarity Selection"
excerpt: "A semantic similarity tool for filtering large Zotero libraries using sentence embeddings."
image: ../images/zss-logo-2.png
logo: /images/zss-logo-2.png
meta: "Python · Zotero"
github: https://github.com/B-Gendron/zotero-similarity-selection
order: 2
author_profile: false
collection: softwares
---

ZSS is a research support tool that helps scholars efficiently filter relevant papers from large Zotero libraries by computing semantic similarity using state-of-the-art sentence embeddings.

## How it works

Given a CSV export of a Zotero library, the tool compares paper titles and abstracts against a user-defined description of the research scope and automatically selects the most relevant entries.

<figure class="sw-fig">
  <img src="{{ '/images/zss-demo-1.png' | relative_url }}" alt="ZSS upload interface">
  <figcaption><strong>Figure 1.</strong> ZSS interface for uploading a Zotero CSV export and defining the research scope description used for semantic similarity comparison.</figcaption>
</figure>

## Results and export

The filtered results can be exported as a CSV file and converted to BibTeX for re-importing into Zotero. The results page provides insights about the selection process, including a similarity distribution histogram to visualize how papers are distributed across similarity scores and where the threshold is.

<figure class="sw-fig">
  <img src="{{ '/images/zss-demo-2.png' | relative_url }}" alt="ZSS results dashboard">
  <figcaption><strong>Figure 2.</strong> Results dashboard showing corpus statistics, similarity threshold, and the distribution of similarity scores.</figcaption>
</figure>
