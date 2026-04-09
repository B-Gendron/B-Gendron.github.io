---
layout: archive
title: "Conversational Control with Ontologies for Large Language Models:
A Lightweight Framework for Constrained Generation"
collection: publications
---

_Gendron & al., 2026_
    
In KG & LLM: Knowledge Graphs and Large Language Models LREC 2026 Workshop, Palma de Mallorca (Spain), May 2026.

<style>
    form button {
        background-color: #4CAF50; /* Green background color */
        color: white; /* White text color */
        padding: 10px 15px; /* Padding inside the button */
        border: none; /* No border */
        border-radius: 5px; /* Rounded corners */
        cursor: pointer; /* Cursor style on hover */
    }

    /* Style for the second button */
    form:nth-child(2) button {
        background-color: #008CBA; /* Blue background color */
    }

     /* Style for the third button */
    form:nth-child(3) button {
        background-color: #A32CC4; /* Purple background color */
    }
</style>

<td>
    <nobr>
<form style="float: left; width=150px; margin-right: 10px" action="https://arxiv.org/abs/2604.04450" method="get" target="_blank"><button type="submit">View on ArXiv</button></form>
<form style="float: left; width=150px; margin-right: 10px" action="https://kg-llm.github.io/program/pdf/2026.kgllmlrec26-1.3.pdf" method="get" target="_blank"><button type="submit">PDF</button></form> 
<form style="float: none; width=150px; margin-right: 10px" action="https://B-Gendron.github.io/files/ref_lrec.txt" method="get" target="_blank"><button type="submit">Cite</button></form>
    </nobr>
</td>

## Abstract

Conversational agents based on Large Language Models (LLMs) have recently emerged as powerful tools for human-computer interaction. Nevertheless, their black-box nature implies challenges in predictability and a lack of personalization, both of which can be addressed by controlled generation. This work proposes an end-to-end method to obtain modular and explainable control over LLM outputs through ontological definitions of aspects related to the conversation. Key aspects are modeled and used as constraints; we then further fine-tune the LLM to generate content accordingly. To validate our approach, we explore two tasks that tackle two key conversational aspects: the English proficiency level and the polarity profile of the content. Using a hybrid fine-tuning procedure on seven state-of-the-art, open-weight conversational LLMs, we show that our method consistently outperforms pre-trained baselines, even on smaller models. Beyond quantitative gains, the framework remains model-agnostic, lightweight, and interpretable, enabling reusable control strategies that can be extended to new domains and interaction goals. This approach enhances alignment with strategy instructions and demonstrates the effectiveness of ontology-driven control in conversational systems. 

*Keywords : ontologies, conversation modeling, large language models, controlled generation*
